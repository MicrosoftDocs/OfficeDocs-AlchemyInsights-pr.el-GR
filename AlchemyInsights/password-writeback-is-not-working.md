---
title: Η Writeback κωδικού πρόσβασης δεν λειτουργεί
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243365"
---
# <a name="password-writeback-is-not-working"></a>Η Writeback κωδικού πρόσβασης δεν λειτουργεί

**Έχω προβλήματα με τη ρύθμιση των παραμέτρων της writeback κωδικού πρόσβασης**

- Η writeback κωδικού πρόσβασης είναι μια εξαιρετική δυνατότητα.
- Βεβαιωθείτε ότι έχετε κατανοήσει τις απαιτήσεις άδειας χρήσης:
  - Πρέπει να έχετε εκχωρήσει τουλάχιστον μία άδεια χρήσης στον οργανισμό σας
  - **Χρήστες μόνο για cloud** - Οποιαδήποτε SKU επί πληρωμή για το Office 365 (O365) ή Azure AD Basic
  - **Χρήστες cloud ή/και** εσωτερικής εγκατάστασης - Azure AD Premium P1 ή P2, Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS) ή Secure Productive Enterprise (SPE)
    - Για να μάθετε περισσότερα σχετικά με τις απαιτήσεις άδειας χρήσης, [ανατρέξτε στις απαιτήσεις παραχώρησης αδειών χρήσης για](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) την επαναφορά κωδικού πρόσβασης από το χρήστη του Azure AD
- Έχετε τουλάχιστον έναν λογαριασμό διαχειριστή και έναν δοκιμαστικό λογαριασμό χρήστη με μία από τις κατάλληλες άδειες χρήσης.
- Πρέπει να συνδέσετε το Azure AD Connect στον πρωτεύοντα emulator ελεγκτή τομέα για να λειτουργήσει η επαναφορά του κωδικού πρόσβασης. Μπορείτε να ρυθμίσετε τις παραμέτρους του Azure AD Connect  ώστε να χρησιμοποιεί έναν πρωτεύοντα ελεγκτή τομέα κάνοντας δεξί κλικ στις ιδιότητες της σύνδεσης συγχρονισμού υπηρεσίας καταλόγου Active Directory και, στη συνέχεια, επιλέγοντας τις παραμέτρους **των διαμερισμάτων καταλόγου.** Από εκεί, αναζητήστε την ενότητα **ρυθμίσεων σύνδεσης ελεγκτή τομέα και επιλέξτε** το πλαίσιο με τίτλο "Να **χρησιμοποιούνται μόνο οι προτιμώμενοι ελεγκτές τομέα".**
  > [!NOTE]
  > Εάν το προτιμώμενο DC δεν είναι ένας emulator PDC, το Azure AD Connect θα εξακολουθεί να έχει πρόσβαση στον PDC για την επαναφορά του κωδικού πρόσβασης.
- Η επαναφορά κωδικού πρόσβασης έχει ρυθμιστεί και ενεργοποιηθεί στο μισθωτή σας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Επιτρέψτε στους χρήστες να επαναφέρουν τους κωδικούς πρόσβασης του Azure AD"](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)που έχουν.
- Βεβαιωθείτε ότι ο λογαριασμός διαχειριστή που χρησιμοποιείται για την ενεργοποίηση της δυνατότητας "Εγγραφή κωδικού πρόσβασης" είναι ένας λογαριασμός διαχειριστή cloud (δημιουργήθηκε στο Azure AD και όχι στο AD εσωτερικής εγκατάστασης)
- Έχετε μια ανάπτυξη μεμονωμένου δάσους AD εσωτερικής εγκατάστασης που εκτελεί Windows Server 2008 R2, Windows Server 2012 ή Windows Server 2012 R2 με εγκατεστημένα τα πιο πρόσφατα service pack
- Έχετε εγκαταστήσει το εργαλείο Azure AD Connect και έχετε προετοιμάσει το περιβάλλον AD για συγχρονισμό στο cloud. Πριν από τη δοκιμή της writeback κωδικού πρόσβασης, βεβαιωθείτε ότι έχετε ολοκληρώσει πρώτα μια πλήρη εισαγωγή και πλήρη συγχρονισμό τόσο από το AD όσο και από το Azure AD στο Azure AD Connect.
- Για να μάθετε περισσότερα, δείτε πώς μπορείτε να κάνετε [πλήρη συγχρονισμό και πλήρη εισαγωγή στο Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**Έχω πρόβλημα με τη συνδεσιμότητα με την επαναφορά κωδικού πρόσβασης**

1. Λήψη και ενεργοποίηση της πιο πρόσφατης έκδοσης του [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Ρύθμιση παραμέτρων τείχους προστασίας: Το εργαλείο Azure AD Connect (1.1.443 και άνω) θα χρειαστεί πρόσβαση **εξερχομένων HTTPS** σε:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Να επιτρέπεται η διατήρηση των αδρανών συνδέσεων για τουλάχιστον 2-3 λεπτά

**Εξακολουθώ να έχω προβλήματα με την επαναφορά του κωδικού πρόσβασης**

- Εάν εξακολουθείτε να αντιμετωπίζετε δυσκολίες, δοκιμάστε να απενεργοποιήσετε και να ενεργοποιήσετε ξανά την υπηρεσία writeback κωδικού πρόσβασης στο εργαλείο Azure AD Connect
- Για να μάθετε περισσότερα, δείτε πώς μπορείτε να [απενεργοποιήσετε και να ενεργοποιήσετε ξανά την writeback κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
