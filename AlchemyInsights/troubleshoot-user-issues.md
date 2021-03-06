---
title: Αντιμετώπιση προβλημάτων χρήστη
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
- "7813"
- "9004358"
ms.openlocfilehash: d9964e50bdea0c41ac14ab3783b579034b5f2c8c
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901037"
---
# <a name="announcements"></a>Ανακοινώσεις

Ακολουθήστε τις οδηγίες της Google σχετικά με τη δοκιμή συμβατότητας για να ελέγξετε εάν επηρεάζονται οι εφαρμογές σας. Οι οδηγίες της Google είναι διαθέσιμες στο https://docs.microsoft.com/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support .

Βεβαιωθείτε ότι χρησιμοποιείτε την προβολή συστήματος Web ή το πρόγραμμα περιήγησης συστήματος κατά την είσοδο στους χρήστες σας με λογαριασμούς Google για καταναλωτές. Για περισσότερες πληροφορίες, ανατρέξτε στο [θέμα προβλήματα κατά την είσοδο στις εφαρμογές χρησιμοποιώντας μόνο το πρόγραμμα περιήγησης Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).


**Δεν μπορώ να δημιουργήσω έναν νέο χρήστη στον κατάλογο του Azure AD**

Για να αντιμετωπίσετε το πρόβλημα ότι δεν μπορείτε να δημιουργήσετε έναν νέο χρήστη στο Azure AD, εκτελέστε τα παρακάτω βήματα:

1. Βεβαιωθείτε ότι έχετε εξουσιοδότηση για τη δημιουργία ενός νέου τυπικού χρήστη. Μόνο ο καθολικός διαχειριστής ή ο ρόλος διαχειριστή χρήστη στο Azure Active Directory (AD) μπορεί να δημιουργήσει έναν νέο τυπικό χρήστη. Εάν δεν είστε σε έναν από αυτούς τους ρόλους, ζητήστε από ένα διαχειριστή να σας προσθέσει σε έναν από αυτούς τους ρόλους ή για να δημιουργήσετε τον νέο λογαριασμό χρήστη για εσάς.
2. Βεβαιωθείτε ότι το όνομα χρήστη βρίσκεται σε έναν τομέα που επαληθεύεται στο Azure AD. Εάν δεν έχετε επαληθευμένα προσαρμοσμένα ονόματα τομέων στο Azure AD, μπορείτε να χρησιμοποιήσετε τον αρχικό τομέα Azure AD, ο οποίος τελειώνει με *. onmicrosoft.com.
3. Βεβαιωθείτε ότι το όνομα χρήστη βρίσκεται σε έναν τομέα ο οποίος δεν είναι ενωμένος με το Azure AD από τη ΔΙΑΦΉΜΙΣΉ σας εσωτερικής εγκατάστασης. Οι χρήστες δεν μπορούν να προστεθούν στο cloud με ονόματα τομέων που είναι ομόσπονδη από εσωτερικής εγκατάστασης.
4. Βεβαιωθείτε ότι κανένας άλλος χρήστης ή επαφή δεν έχει ήδη το όνομα χρήστη που θέλετε να εκχωρήσετε στο νέο χρήστη. Τα ονόματα χρηστών πρέπει να είναι μοναδικά σε όλο το Azure AD.
5. Ανατρέξτε στο θέμα [ρόλοι και διαχειριστές του Azure AD](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) για τη διαφήμισή σας Azure.
6. Ανατρέξτε στα [ονόματα τομέων](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Domains) για τη διαφήμισή σας Azure.
7. Εξετάστε τα [αρχεία καταγραφής ελέγχου](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Audit) για να δείτε πιο λεπτομερείς πληροφορίες σχετικά με έναν χρήστη που δημιουργήθηκε πρόσφατα ή διαγράφηκε, όπως ο οποίος πραγματοποίησε την ενέργεια και πότε.
8. Για περισσότερες πληροφορίες σχετικά με την προσθήκη νέων χρηστών, ανατρέξτε στο θέμα [χρήση της πύλης Azure για τη δημιουργία νέου χρήστη στο Azure AD](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) .
9. Για περισσότερες πληροφορίες σχετικά με τα δικαιώματα ρόλου διαχειριστή στο Azure AD, ανατρέξτε στο θέμα [ρόλοι διαχείρισης του Azure AD](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference).
10. Για λεπτομέρειες σχετικά με τη δημιουργία ενός χρήστη χρησιμοποιώντας το Azure AD PowerShell, ανατρέξτε [στο θέμα Azure AD PowerShell για να δημιουργήσετε έναν νέο χρήστη](https://docs.microsoft.com/powershell/module/azuread/new-azureaduser).

**Πρόβλημα με την εγγραφή από το χρήστη**

Για να αντιμετωπίσετε προβλήματα σχετικά με την εγγραφή από το χρήστη, ακολουθήστε τα παρακάτω βήματα:

1. Για να χρησιμοποιήσετε την εγγραφή από το χρήστη με τις εφαρμογές σας, ενεργοποιήστε πρώτα την εγγραφή από το χρήστη για τον μισθωτή σας. 
2. Για να ενεργοποιήσετε μια εφαρμογή για την υποστήριξη της εγγραφής από το χρήστη, προσθέστε την στη ροή χρήστη σας. Την επόμενη φορά που θα μεταβείτε στη σελίδα σύνδεσης για τη συγκεκριμένη εφαρμογή, θα δείτε μια επιλογή **_χωρίς λογαριασμό; Δημιουργήστε ένα!_* _. Αυτή η ενέργεια ξεκινά τη διαδικασία εγγραφής από το χρήστη.
3. Για πληροφορίες σχετικά με τον τρόπο χρήσης της εγγραφής από το χρήστη για τη συμπλήρωση μιας εταιρείας στο Azure AD, ανατρέξτε στο θέμα εγγραφή από το [χρήστη για το Azure AD](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-self-service-signup).
4. Αφού συσχετίσετε τη ροή χρήστη με μία ή περισσότερες εφαρμογές, οι χρήστες που επισκέπτονται αυτήν την εφαρμογή θα έχουν τη δυνατότητα να εγγραφούν και να κερδίσουν έναν λογαριασμό επισκέπτη χρησιμοποιώντας τις επιλογές που έχουν ρυθμιστεί στη ροή του χρήστη. Για περισσότερες πληροφορίες σχετικά με την εγγραφή και την απόκτηση ενός λογαριασμού επισκέπτη, οι χρήστες μπορούν να δουν την εγγραφή από το χρήστη [για τους χρήστες](https://docs.microsoft.com/azure/active-directory/external-identities/self-service-sign-up-user-flow).

_ *Πρόβλημα προσκαλώντας έναν εξωτερικό χρήστη**

Για την αντιμετώπιση προβλημάτων σχετικά με την πρόσκληση ενός εξωτερικού χρήστη, εκτελέστε το παρακάτω βήμα:

Βεβαιωθείτε ότι στέλνετε μια πρόσκληση ενός χρήστη στη διεύθυνση ηλεκτρονικού ταχυδρομείου που ταιριάζει με το όνομα με το οποίο συνδέεται ο χρήστης. Εάν στείλετε την πρόσκληση στη διεύθυνση ηλεκτρονικού ταχυδρομείου του διακομιστή μεσολάβησης ενός χρήστη, ο χρήστης δεν μπορεί να την εξαργυρώσει. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [τεκμηρίωση του Azure AD B2B](https://docs.microsoft.com/azure/active-directory/external-identities/).

**Δεν μπορώ να αναθέτω άδειες χρήσης σε ένα χρήστη**

Για την αντιμετώπιση προβλημάτων σχετικά με την εκχώρηση αδειών χρήσης σε ένα χρήστη, εκτελέστε τα παρακάτω βήματα:

1. Για να διαχειριστείτε τις άδειες χρήσης, βεβαιωθείτε ότι χρησιμοποιείτε ένα λογαριασμό με έναν από τους απαιτούμενους ρόλους διαχειριστή: καθολικός διαχειριστής, διαχειριστής άδειας χρήσης ή διαχειριστής χρήστη. Μπορείτε να επιλέξετε το ρόλο του χρήστη στην καρτέλα " **ρόλος καταλόγου** " στη λεπίδα του χρήστη.
2. Εάν χρησιμοποιείτε την πύλη Azure και η εκχώρηση αδειών χρήσης αποτυγχάνει, κάντε κλικ στην ειδοποίηση στην επάνω δεξιά γωνία. Αυτό ανοίγει μια λεπίδα με λεπτομέρειες σχετικά με το τι πήγε στραβά. Στις περισσότερες περιπτώσεις, αυτό αρκεί για να κατανοήσετε και να επιλύσετε το πρόβλημα.
3. Για να μπορέσει να εκχωρηθεί μια άδεια χρήσης σε ένα χρήστη, βεβαιωθείτε ότι η ιδιότητα **θέση χρήσης** έχει οριστεί για το χρήστη. Επαληθεύστε ότι ο χρήστης έχει ρυθμίσει αυτή την ιδιότητα, προβάλλοντας την καρτέλα **προφίλ** στη λεπίδα του χρήστη.
4. Βεβαιωθείτε ότι υπάρχουν αρκετές διαθέσιμες άδειες χρήσης για το προϊόν που προσπαθείτε να εκχωρήσετε. Μπορείτε να δείτε τον αριθμό των διαθέσιμων αδειών χρήσης στην πύλη Azure, στο [Azure Active Directory-> άδειες χρήσης-> όλα τα προϊόντα](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/LicensesMenuBlade/Products).
5. Ο χρήστης μπορεί να έχει ήδη μια άλλη άδεια χρήσης των οποίων οι υπηρεσίες έρχονται σε διένεξη με εκείνες στη νέα άδεια χρήσης που προσπαθείτε να εκχωρήσετε. Για παράδειγμα, εάν ο χρήστης έχει ενεργοποιημένη την υπηρεσία Exchange Online (πρόγραμμα 1), δεν θα μπορείτε να εκχωρήσετε μια άδεια χρήσης με το Exchange Online (πρόγραμμα 2). Απενεργοποιήστε μία από τις υπηρεσίες για να επιτρέψετε τη νέα εκχώρηση άδειας χρήσης. Εάν χρησιμοποιείτε τα cmdlet του Azure Portal ή PowerShell, η σελίδα " **Λεπτομέρειες προβλήματος** " παραθέτει τις συγκεκριμένες υπηρεσίες που προκαλούν τη διένεξη.
6. Εάν προσπαθείτε να καταργήσετε μια άδεια χρήσης και η οποία αποτυγχάνει, ο χρήστης μπορεί να έχει άλλες άδειες χρήσης με υπηρεσίες που εξαρτώνται από τις υπηρεσίες που προσπαθείτε να καταργήσετε. Εάν χρησιμοποιείτε τα cmdlet του Azure Portal ή PowerShell, το μήνυμα σφάλματος θα παραθέσετε τις συγκεκριμένες υπηρεσίες που έχουν εξαρτήσεις.
7. Εάν θέλετε να καταλάβετε γιατί προστέθηκε/καταργήθηκε μια άδεια χρήσης από ένα χρήστη (για παράδειγμα, ποιος άλλος στην εταιρεία σας μπορεί να έχει κάνει αλλαγές), ελέγξτε τα αρχεία καταγραφής ελέγχου. Ορίστε το φίλτρο σε **δραστηριότητες άδειας χρήσης** για την εμφάνιση όλων των τροποποιήσεων, συμπεριλαμβανομένου του "δράστη" που τα πραγματοποίησε.
8. Εάν χρησιμοποιείτε το Exchange Online, ορισμένοι χρήστες στο μισθωτή σας ενδέχεται να έχουν εσφαλμένη ρύθμιση παραμέτρων με την ίδια τιμή διεύθυνσης διακομιστή μεσολάβησης. Σε αυτές τις περιπτώσεις, ενδέχεται να εμφανιστούν γενικά μηνύματα σφάλματος όταν αποτύχει μια λειτουργία άδειας χρήσης. [Αυτό το άρθρο](https://docs.microsoft.com/exchange/troubleshoot/administration/proxy-address-being-used) περιέχει περισσότερες πληροφορίες σχετικά με αυτό το πρόβλημα, συμπεριλαμβανομένων των πληροφοριών σχετικά με τον [τρόπο σύνδεσης στο Exchange Online με χρήση απομακρυσμένου PowerShell](https://docs.microsoft.com/powershell/exchange/connect-to-exchange-online-powershell). Για να προσδιορίσετε ποιοι χρήστες του μισθωτή σας, περιέχουν την ίδια διεύθυνση διακομιστή μεσολάβησης, εκτελέστε αυτό το cmdlet του Exchange Online:

Εκτέλεση

Get-Recipient | όπου {$ _. EmailAddresses-Match <user principal name> } | fL name, RecipientType, emailaddresses





