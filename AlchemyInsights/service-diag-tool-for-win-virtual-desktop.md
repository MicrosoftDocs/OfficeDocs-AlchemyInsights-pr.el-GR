---
title: Εργαλείο διαγνωστικών υπηρεσιών για την εικονική επιφάνεια εργασίας των Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003893"
- "6947"
ms.openlocfilehash: c2e6f7fbcddc6721425840e87202a165cdb22664
ms.sourcegitcommit: 87bf574162e536003164ff9af50005c5a7dce601
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/14/2020
ms.locfileid: "49678619"
---
# <a name="service-diagnostics-tool-for-windows-virtual-desktop"></a>Εργαλείο διαγνωστικών υπηρεσιών για την εικονική επιφάνεια εργασίας των Windows

Το Windows Virtual Desktop (WVD) προσφέρει ένα διαγνωστικό εργαλείο που επιτρέπει στους διαχειριστές να εντοπίζουν σφάλματα μέσω μιας μεμονωμένης διασύνδεσης. Αυτό το εργαλείο καταγράφει πληροφορίες που σχετίζονται με τα διαγνωστικά κάθε φορά που χρησιμοποιείται το WVD από κάποιον που έχει εκχωρήσει ένα ρόλο WVD. Κάθε αρχείο καταγραφής περιέχει πληροφορίες σχετικά με το ρόλο του WVD που εμπλέκεται στη δραστηριότητα, τα μηνύματα σφάλματος που εμφανίζονται κατά τη διάρκεια της περιόδου λειτουργίας και τις πληροφορίες σχετικά με τον μισθωτή και το χρήστη. Η ανάλυση του αρχείου καταγραφής Azure μπορεί να ρυθμιστεί για την καταγραφή του αρχείου καταγραφής δραστηριοτήτων που δημιουργήθηκε από το εργαλείο διάγνωσης. Αυτό μπορεί να γίνει ως εξής:

1. Δημιουργήστε ένα χώρο εργασίας του αρχείου καταγραφής ανάλυσης με την [πύλη Azure](https://go.microsoft.com/fwlink/?linkid=2129500) ή το [Azure PowerShell](https://go.microsoft.com/fwlink/?linkid=2129501).
1. [Συνδέστε τους υπολογιστές με Windows στην οθόνη Azure](https://go.microsoft.com/fwlink/?linkid=2129913). Λήψη του ΑΝΑΓΝΩΡΙΣΤΙΚού χώρου εργασίας και του πρωτεύοντος κλειδιού του χώρου εργασίας σας. Ο οδηγός εγκατάστασης χρειάζεται αυτές τις πληροφορίες για να ρυθμίσει σωστά τις παραμέτρους του παράγοντα και να εξασφαλίσει ότι μπορεί να επικοινωνεί με την οθόνη Azure.
1. [Σπρώξτε τα δεδομένα διαγνωστικών στο χώρο εργασίας σας](https://go.microsoft.com/fwlink/?linkid=2128284). Μπορείτε να πιέσετε τα διαγνωστικά δεδομένα από τον μισθωτή του WVD στην ανάλυση καταγραφής για το χώρο εργασίας σας.
1. [Προσδιορίστε και Διαγνώστε προβλήματα](https://go.microsoft.com/fwlink/?linkid=2128338) που είναι εσωτερικά ή εξωτερικά σε σχέση με το WVD.

Για να μάθετε περισσότερα σχετικά με τη ρύθμιση παραμέτρων του εργαλείου διαγνωστικών υπηρεσιών για το WVD, ανατρέξτε στο θέμα [χρήση της ανάλυσης καταγραφής για τη δυνατότητα διαγνωστικών](https://go.microsoft.com/fwlink/?linkid=2128084).
