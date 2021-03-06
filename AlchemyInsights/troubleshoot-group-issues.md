---
title: Αντιμετώπιση προβλημάτων ομάδας
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7814"
- "9004358"
ms.openlocfilehash: 7e2957a27305e8fb0bfd10e21189cef9870c5aaa
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "50713646"
---
# <a name="troubleshoot-group-issues"></a>Αντιμετώπιση προβλημάτων ομάδας

**Πρέπει να εκχωρήσω μια ομάδα σε έναν ρόλο Azure AD**

Για να εκχωρήσετε μια ομάδα του Azure Active Directory (AD) σε ένα ρόλο azure AD, εκτελέστε τα ακόλουθα βήματα:

1. Δημιουργία νέας ομάδας - Για να δημιουργήσετε μια νέα ομάδα:

    a. Πραγματοποιήστε είσοδο στο κέντρο διαχείρισης του Azure AD με δικαιώματα διαχειριστή ρόλων ή καθολικών δικαιωμάτων διαχειριστή. 
    b. Επιλέξτε Azure Active Directory για > ομάδες > όλες τις > Νέα ομάδα. 
    c. Δημιουργήστε την ομάδα.

2. Αναθέστε το ρόλο στην ομάδα είτε κατά τη δημιουργία της ομάδας είτε μετά τη δημιουργία της ομάδας.

    a. Για να αναθέσετε έναν ρόλο στην ομάδα κατά τη δημιουργία της ομάδας, ενεργοποιήστε την εναλλαγή μεταξύ ρόλων Azure AD και δημιουργήστε την ομάδα.
    b. Για να αναθέσετε ένα ρόλο στην ομάδα μετά τη δημιουργία του, μεταβείτε στην καρτέλα "Ανάθεση ρόλων" για την ομάδα που μόλις δημιουργήσατε και αναθέστε το ρόλο στην ομάδα.

**Πρέπει να διαχειριστώ την ιδιότητα μέλους μιας ομάδας στην οποία έχει εκχωρηθεί ο ρόλος azure AD**

1. Για να αποτρέψετε την ανύψωση των δικαιωμάτων, από προεπιλογή, μόνο ο διαχειριστής με δικαιώματα και ο καθολικός διαχειριστής μπορούν να τροποποιήσουν την ιδιότητα μέλους μιας ομάδας στην οποία έχει εκχωρηθεί ένας ρόλος. Ωστόσο, μπορούν να επιλέξουν να αναθέσουν έναν κάτοχο για μια τέτοια ομάδα και να αναθέσουν αυτήν την εργασία. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα, Χρησιμοποιήστε ομάδες cloud για τη διαχείριση αναθέσεων ρόλων στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/roles/groups-concept)
2. Για συνήθεις ερωτήσεις και συμβουλές αντιμετώπισης προβλημάτων για την ανάθεση ρόλων σε ομάδες στο Azure AD, ανατρέξτε στο θέμα "Αντιμετώπιση προβλημάτων ρόλων [που έχουν εκχωρηθεί σε ομάδες cloud".](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting)

**Δυναμικές ομάδες**

1. Εάν δεν μπορείτε να βρείτε τα ενσωματωμένα χαρακτηριστικά χρήστη, βεβαιωθείτε ότι το χαρακτηριστικό βρίσκεται στη λίστα των υποστηριζόμενων ιδιοτήτων.
2. Εάν αναζητάτε ενσωματωμένα χαρακτηριστικά συσκευής, βεβαιωθείτε ότι το χαρακτηριστικό βρίσκεται στη λίστα των χαρακτηριστικών της συσκευής 
3. Εκτός από τα ενσωματωμένα χαρακτηριστικά χρήστη και συσκευής, μπορείτε επίσης να χρησιμοποιήσετε [χαρακτηριστικά επέκτασης.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership#extension-properties-and-custom-extension-properties) Μετά το συγχρονισμό χαρακτηριστικών επέκτασης από τον Windows Server AD εσωτερικής εγκατάστασης ή από μια συνδεδεμένη εφαρμογή SaaS, τα χαρακτηριστικά θα πρέπει να είναι ορατά στην αναπτυσσόμενη λίστα της δόμησης κανόνων. Μπορείτε να βρείτε το προσαρμοσμένο όνομα χαρακτηριστικού στον κατάλογο κάνοντας ερώτημα για το χαρακτηριστικό ενός χρήστη χρησιμοποιώντας το PowerShell και κάνοντας αναζήτηση για το όνομα του χαρακτηριστικού. Αυτά θα μπορούσαν επίσης να χρησιμοποιηθούν κατά τη δημιουργία κανόνων στη σύνταξη κανόνων.
4. Βεβαιωθείτε ότι ο μισθωτής σας έχει την κατάλληλη άδεια χρήσης. Για τις δυναμικές ομάδες, ο μισθωτής πρέπει να έχει άδεια χρήσης του Azure AD P1 Premium. Μπορείτε να αποκτήσετε πρόσβαση στη λίστα των προγραμμάτων άδειας χρήσης του Azure AD [εδώ.](https://azure.microsoft.com/pricing/details/active-directory/) Μπορείτε να αποκτήσετε πρόσβαση στα προγράμματα παραχώρησης αδειών χρήσης για τη Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια [εδώ.](https://www.microsoft.com/microsoft-365/enterprise-mobility-security/compare-plans-and-pricing)
5. Βεβαιωθείτε ότι ο ρόλος του χρήστη που δημιουργεί τη δυναμική ομάδα είναι ένας καθολικός διαχειριστής, διαχειριστής intune, διαχειριστής ομάδας ή διαχειριστής χρήστη.
6. Περιμένετε να συμπληρωθεί η ομάδα. Ανάλογα με το μέγεθος του μισθωτή σας, η ομάδα μπορεί να χρειαστεί έως και 24 ώρες για να συμπληρωθεί για πρώτη φορά ή μετά την αλλαγή ενός κανόνα.
7. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Δημιουργία κανόνων που βασίζονται σε χαρακτηριστικά για τη δυναμική ιδιότητα μέλους ομάδας".](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-dynamic-membership)

**Πρέπει να διαγράψω μια ομάδα**

1. Οι ομάδες μπορούν να διαγραφούν από τον κατάλογο χρησιμοποιώντας Remove-AzureADGroup cmdlet στη λειτουργική μονάδα Azure AD Powershell.
2. Πριν προσπαθήσετε να διαγράψετε μια συγχρονισμένη ομάδα στο Azure AD, βεβαιωθείτε ότι έχετε διαγράψει όλες τις άδειες χρήσης που έχουν εκχωρηθεί για να αποφύγετε τα σφάλματα.
3. Για περισσότερες πληροφορίες σχετικά με τη διαγραφή ομάδων, [ανατρέξτε στο θέμα Διαγραφή ομάδας με εκχωρηθείσα άδεια χρήσης.](https://docs.microsoft.com/azure/active-directory/enterprise-users/licensing-group-advanced#deleting-a-group-with-an-assigned-license)

**Θέλω να επαναφέρω μια διαγραμμένη ομάδα**

1. Εάν διαγραφεί μια ομάδα του Office 365, είναι δυνατή η επαναφορά της μόνο 30 ημέρες πριν από την οριστική διαγραφή. Μετά την οριστική διαγραφή, δεν είναι πλέον δυνατό να αποκατασταθεί η ομάδα. Μάθετε περισσότερα σχετικά με την επαναφορά ομάδων [εδώ.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)
2. Αυτή η λειτουργία δεν υποστηρίζεται για ομάδες ασφαλείας και ομάδες διανομής.
3. Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για την επαναφορά μιας ομάδας του Office 365. Οι καθολικοί διαχειριστές, οι διαχειριστές ομάδων, οι διαχειριστές λογαριασμών χρηστών, οι διαχειριστές υπηρεσιών intune, η υποστήριξη συνεργάτη επιπέδου 1 ή επιπέδου2 και ο κάτοχος της ομάδας μπορούν να επαναφέρουν μια ομάδα.
4. Όταν διαγράφεται και αποκαταστάθηκε μια δυναμική ομάδα, αυτή θεωρείται ως νέα ομάδα και συμπληρώνεται εκ νέου σύμφωνα με τον κανόνα. Αυτή η διαδικασία μπορεί να διαρκέσει έως και 24 ώρες.
5. Για περισσότερες πληροφορίες σχετικά με την επαναφορά μιας διαγραμμένης ομάδας, ανατρέξτε στο θέμα ["Επαναφορά διαγραμμένης ομάδας του Office 365 στο Azure Active Directory".](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Ρύθμιση παραμέτρων πολιτικής λήξης ομάδας**

1. Αυτή η λειτουργικότητα υποστηρίζεται μόνο για ομάδες του Office 365 και όχι για ομάδες ασφαλείας και ομάδες διανομής δεν υποστηρίζεται.
2. Η ρύθμιση παραμέτρων και η χρήση της πολιτικής λήξης για ομάδες του Office 365 απαιτεί άδεια χρήσης του Azure AD Premium.
3. Προς το παρόν, μόνο μία πολιτική λήξης μπορεί να ρυθμιστεί για ομάδες του Office 365 σε ένα μισθωτή.
4. Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές ομάδων, οι διαχειριστές χρηστών και ο κάτοχος της ομάδας μπορούν να ανανεώσουν μια ομάδα.
5. Εάν μια ομάδα του Office 365 έχει λήξει, διαγράφεται και μπορεί να αποκατασταθεί μόνο 30 ημέρες πριν από την οριστική διαγραφή. Μετά την οριστική διαγραφή, δεν είναι πλέον δυνατό να αποκατασταθεί η ομάδα. Μάθετε περισσότερα σχετικά με την επαναφορά ομάδων [εδώ.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Αυτόματη ανανέωση βάσει δραστηριότητας**

Οι δραστηριότητες χρηστών από το SharePoint, το Outlook και το Teams μπορούν να ενεργοποιήσουν την αυτόματη ανανέωση ομάδων. Οι δραστηριότητες ελέγχονται 35 ημέρες πριν από τη λήξη μιας ομάδας. Εάν υπάρχει δραστηριότητα κατά τη διάρκεια του τρέχοντος κύκλου ζωής ομάδας, η ομάδα θα ανανεωθεί αυτόματα και η ειδοποίηση μέσω ηλεκτρονικού ταχυδρομείου δεν θα σταλεί στους κατόχους της ομάδας.

**Χρονισμός ειδοποιήσεων για ομάδες που έχουν λήξει**

1. Οι ειδοποιήσεις ηλεκτρονικού ταχυδρομείου αποστέλλονται στους κατόχους ομάδας του Office 365 30 ημέρες, 15 ημέρες και 1 ημέρα πριν από τη λήξη της ομάδας.
2. Όταν ορίζετε για πρώτη φορά τη λήξη, οι ομάδες που είναι παλαιότερες από το χρονικό διάστημα λήξης ορίζονται σε 35 ημέρες μέχρι τη λήξη.
3. Η ημερομηνία λήξης της ομάδας υπολογίζεται με βάση την ημερομηνία ανανέωσης της ομάδας και όχι με βάση την ημερομηνία ενημέρωσης της πολιτικής. Εάν η πολιτική λήξης ενημερωθεί, η ημερομηνία λήξης δεν θα αλλάξει.
4. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα ,Μηνύματα ηλεκτρονικού](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-lifecycle) ταχυδρομείου πολιτικής λήξης και ανανέωσης ομάδας και Επαναφορά [διαγραμμένης ομάδας του Office 365 στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-restore-deleted)

**Δικαίωμα δημιουργίας ομάδας**

Βεβαιωθείτε ότι είστε εξουσιοδοτημένοι για τη δημιουργία μιας νέας ομάδας. Οι καθολικοί διαχειριστές μπορούν να απενεργοποιήσουν τη δημιουργία ομάδας στην πύλη Azure ή στον Πίνακα πρόσβασης. Μπορεί να χρειαστείτε ένα διαχειριστή για να δημιουργήσετε τη νέα ομάδα για εσάς ή να σας δώσει τα κατάλληλα δικαιώματα.

1. [Δημιουργία νέας ομάδας και προσθήκη μελών στην πύλη Azure](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-groups-create-azure-portal)
2. [Δημιουργία ομάδων στο Powershell MSOnline](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#create-groups)
3. [Απενεργοποίηση δημιουργίας ομάδων στο Powershell](https://docs.microsoft.com/azure/active-directory/enterprise-users/groups-settings-v2-cmdlets#disable-group-creation-by-your-users) 
4. [Διαχείριση των χρηστών που μπορούν να δημιουργούν ομάδες στο Office 365](https://docs.microsoft.com/microsoft-365/solutions/manage-creation-of-groups) 
5. [Απενεργοποίηση ειδοποίησης υποδοχής του Office 365 μέσω Powershell](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)
6. [Ρόλοι διαχείρισης του Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)

**Διαχείριση δικαιωμάτων δημιουργίας ομάδας**

1. Οι καθολικοί διαχειριστές μπορούν να διαχειριστούν τα δικαιώματα δημιουργίας ομάδων για την ασφάλεια ή τις ομάδες του Office 365 που έχουν δημιουργηθεί στην πύλη Azure ή στον Πίνακα πρόσβασης, ορίζοντας τη δυνατότητα "Οι χρήστες μπορούν να δημιουργήσουν ομάδες ασφαλείας στις πύλες **Azure"** ή οι χρήστες μπορούν να δημιουργήσουν ομάδες του **Office 365** στις ρυθμίσεις πυλών Azure σε όλες τις ομάδες > Γενικά **(Ρυθμίσεις).**
2. Μπορείτε επίσης να περιορίσετε τη δημιουργία ομάδων για να επιλέξετε μια ομάδα χρηστών, εάν έχετε μια άδεια χρήσης azure AD P1 Premium.

**Απενεργοποίηση ειδοποίησης υποδοχής για νέα μέλη μιας ομάδας του Office 365**

Η ειδοποίηση υποδοχής που αποστέλλεται στους χρήστες που έχουν προστεθεί σε ομάδες του Office 365 μπορεί να απενεργοποιηθεί, ορίζοντας `UnifiedGroupWelcomeMessageEnabled` την τιμή **False** στο Powershell. Μάθετε περισσότερα σχετικά με αυτήν τη [ρύθμιση εδώ.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup)













