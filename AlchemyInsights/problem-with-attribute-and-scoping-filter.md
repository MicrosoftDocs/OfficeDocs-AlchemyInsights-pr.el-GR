---
title: Πρόβλημα με το χαρακτηριστικό και το φίλτρο αναζήτησης
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8470"
- "9004687"
ms.openlocfilehash: 78df24c0d8a670d678e26879cf81476f1ae9b92d
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481366"
---
# <a name="problem-with-attribute-and-scoping-filter"></a>Πρόβλημα με το χαρακτηριστικό και το φίλτρο αναζήτησης

**Πρόβλημα με αντικρουόμενες τιμές UPN**

Η εργάσιμη ημέρα σε AD User Provisioning Workday to AD User Provisioning εμφανίζει το μήνυμα σφάλματος **HybridSynchronizationActiveDirectoryUserPrincipalNameNotUnique.** Η λειτουργία απέτυχε, επειδή η τιμή UPN που παρέχεται για την προσθήκη/τροποποίηση δεν είναι μοναδική σε όλο το δάσος. Λεπτομέρειες σφάλματος: **CONSTRAINT_ATT_TYPE - userPrincipalName.**

Η **τιμή userPrincipalName** που προσπαθεί να ορίσει η γραμμή σύνδεσης Workday κατά τη δημιουργία του λογαριασμού χρήστη AD υπάρχει ήδη στον τομέα AD προορισμού. Αυτό σημαίνει ότι είτε (1) ο χρήστης υπάρχει ήδη και ο έλεγχος αναγνωριστικού που ταιριάζει απέτυχε για το χρήστη είτε (2) ο κανόνας δημιουργίας UPN δημιούργησε μια τιμή σε διένεξη.

Ακολουθούν τα προτεινόμενα βήματα επίλυσης:

Εάν ο χρήστης υπάρχει ήδη και ο έλεγχος αναγνωριστικού που ταιριάζει απέτυχε να συνδέσει το λογαριασμό Εργάσιμη ημέρα με το λογαριασμό της υπηρεσίας καταλόγου Active Directory, ελέγξτε εάν το χαρακτηριστικό αναγνωριστικού που ταιριάζει (συνήθως **αναγνωριστικό** υπαλλήλου) τόσο στην εργάσιμη ημέρα όσο και στο AD έχει ακριβή αντιστοιχία. Εάν δεν υπάρχει αντιστοιχία, αυτό είναι ένα πρόβλημα με τα δεδομένα που πρέπει να διορθωθεί. Για παράδειγμα, εάν το αναγνωριστικό υπαλλήλου στο Workday είναι 001052 και στο AD είναι 1052, ο μηχανισμός προμήθειας δεν θα συνδέσει τους δύο λογαριασμούς και θα προσπαθήσει να δημιουργήσει ένα χρήστη που υπάρχει ήδη. Η λύση σε αυτή την περίπτωση είναι να αλλάξετε την τιμή **"EmployeeID"** στο AD ώστε να περιλαμβάνει τα αρχικά μηδενικά ώστε να είναι 001052.
Εάν η παράσταση δημιουργίας UPN δεν δημιουργεί μια μοναδική τιμή, εξετάστε το ενδεχόμενο να χρησιμοποιήσετε τη συνάρτηση απο-δημιουργίας **SelectUniqueValue** για να δημιουργείτε μια μοναδική τιμή κάθε φορά.

**Η εργάσιμη ημέρα σε προμήθεια χρήστη AD δεν έχει ορίσει τιμή χαρακτηριστικού διαχειριστή για το λογαριασμό χρήστη AD**

Η εργασία "Εργασία σε παροχή χρήστη AD" δεν καθορίζει την τιμή χαρακτηριστικού **διαχειριστή** για τους λογαριασμούς χρηστών AD. Υπάρχουν δύο πιθανά σενάρια όταν παρουσιάζεται αυτή η συμπεριφορά:

1. Ο διευθυντής σε Εργάσιμη ημέρα δεν μπορεί να επιλυθεί σε έναν αντίστοιχο λογαριασμό χρήστη AD, επειδή ο διευθυντής δεν έχει εμβέλεια.
2. Σε ένα **σενάριο πολλών τομέων AD,** η διαχείριση της εργάσιμης ημέρας δεν υπάρχει στον ίδιο τομέα με το χρήστη.

Δοκιμάστε τα παρακάτω βήματα για να επιλύσετε το πρόβλημα:

1. Εάν έχετε ορίσει φίλτρα εμβέλειας, ελέγξτε πρώτα εάν ο διευθυντής έχει εμβέλεια και ότι ικανοποιεί τον όρο εμβέλειας. Εάν ο διευθυντής δεν ικανοποιεί το φίλτρο εμβέλειας, αλλάξτε το φίλτρο, ώστε ο διευθυντής να έχει επίσης πεδίο εφαρμογής της λειτουργίας παροχής.
2. Εάν έχετε πολλούς τομείς AD, τότε η σύνδεση έχει έναν γνωστό περιορισμό αδυναμίας επίλυσης αναφορών μεταξύ τομέων.

Για περισσότερες λεπτομέρειες σχετικά με τη ρύθμιση παραμέτρων της εργάσιμης ημέρας για την αυτοματοποιημένη παροχή, ανατρέξτε στο πρόγραμμα εκμάθησης: Ρύθμιση [παραμέτρων εργάσιμης ημέρας για αυτόματη προμήθεια από χρήστες.](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)













