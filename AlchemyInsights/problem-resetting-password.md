---
title: Πρόβλημα με την επαναφορά κωδικού πρόσβασης
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "9360"
ms.openlocfilehash: aa1eba1efef6a4c28aa6b9229071304093395922
ms.sourcegitcommit: 9a00005546c2fe473e3cea2b06e38c27eada88c4
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694375"
---
# <a name="problems-resetting-password"></a>Προβλήματα με την επαναφορά κωδικού πρόσβασης

Ακολουθούν ορισμένα από τα προβλήματα που ενδέχεται να αντιμετωπίσουν κατά την επαναφορά του κωδικού πρόσβασης και οι πιθανές λύσεις:

**I'm having an issue with password reset not covered in the other categories**

- Βεβαιωθείτε ότι έχετε την άδεια να επαναφέρετε τους κωδικούς πρόσβασης. Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών. Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.
- Βεβαιωθείτε ότι έχετε κατανοήσει τις απαιτήσεις άδειας χρήσης:
    - Πρέπει να έχετε τουλάχιστον μία άδεια χρήσης εκχωρήθηκε στον οργανισμό σας
        - Μόνο για χρήστες cloud - Οποιαδήποτε SKU επί πληρωμή για το Office 365 (O365) ή Azure AD Basic
        - Χρήστες cloud ή/και εσωτερικής εγκατάστασης - Azure AD Premium P1 ή P2, Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS) ή Secure Productive Enterprise (SPE)
        - Για να διαβάσετε περισσότερα σχετικά με τις απαιτήσεις άδειας χρήσης, ανατρέξτε στο άρθρο ["Απαιτήσεις παραχώρησης αδειών χρήσης" για](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)την επαναφορά κωδικού πρόσβασης από το χρήστη του Azure AD.

**Έχω προβλήματα με τη δοκιμή της πολιτικής επαναφοράς κωδικού πρόσβασης που ορίζετε**

- Οι πολιτικές που εφαρμόστηκαν πρόσφατα μπορεί να διαρκέσει αρκετά λεπτά για να αναπαραχθούν σε όλα τα κέντρα δεδομένων και τα τελικά σημεία. Η φυσική απόσταση από το κέντρο δεδομένων θα επηρεάσει επίσης το πόσο γρήγορα εφαρμόζονται οι αλλαγές.
- Δοκιμή με έναν τελικό χρήστη και όχι με διαχειριστή και πιλοτική χρήση με ένα μικρό σύνολο χρηστών. Οι πολιτικές που έχουν ρυθμιστεί στην πύλη Azure ισχύουν ΜΟΝΟ για τελικούς χρήστες και όχι για διαχειριστές. Η Microsoft επιβάλλει μια ισχυρή προεπιλεγμένη πολιτική επαναφοράς κωδικού πρόσβασης δύο πυλών για οποιονδήποτε ρόλο διαχειριστή Azure (Παράδειγμα: Καθολικός διαχειριστής, Διαχειριστής υπηρεσίας βοήθειας, Διαχειριστής κωδικών πρόσβασης κ.λπ.)
    - Μάθετε περισσότερα σχετικά με [τις πολιτικές για διαχειριστές.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)

**Θέλω να αναπτύξω την επαναφορά κωδικού πρόσβασης, αλλά δεν θέλω να κάνω τους χρήστες μου να καταχωρήσουν πρόσθετες πληροφορίες ασφάλειας**

Συμπληρώστε εκ των προ-συμπληρωμένα δεδομένα για τους χρήστες σας, ώστε να μην χρειάζεται να το κάνουν! - Ως διαχειριστής, μπορείτε να ορίσετε τις ιδιότητες τηλεφώνου και ηλεκτρονικού ταχυδρομείου για τους χρήστες σας πριν από την επαναφορά του κωδικού πρόσβασης στον οργανισμό σας. Μπορείτε να το κάνετε αυτό χρησιμοποιώντας ένα API, το PowerShell ή το Azure AD Connect. Περισσότερες πληροφορίες εδώ:
- [Ανάπτυξη επαναφοράς κωδικού πρόσβασης χωρίς να απαιτείται καταχώρηση από τους χρήστες](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-password-policy-differences)
- [Ποια δεδομένα χρησιμοποιούνται από την επαναφορά κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Το κουμπί επαναφοράς κωδικού πρόσβασης είναι γκριζαρισμένο**

Δεν έχετε εξουσιοδότηση να επαναφέρετε τους κωδικούς πρόσβασης αυτού του χρήστη. Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών. Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.

**Δεν βλέπω το δίσκο επαναφοράς κωδικού πρόσβασης**

Δεν έχετε εξουσιοδότηση για την επαναφορά κωδικών πρόσβασης. Μόνο οι καθολικοί διαχειριστές, οι διαχειριστές κωδικών πρόσβασης και οι διαχειριστές χρηστών μπορούν να επαναφέρουν τους κωδικούς πρόσβασης των χρηστών. Οι καθολικοί διαχειριστές μπορούν επίσης να επαναφέρουν τους κωδικούς πρόσβασης άλλου διαχειριστή με δικαιώματα.

**Δεν βλέπω το blade ενοποίησης εσωτερικής εγκατάστασης κατά την επαναφορά κωδικού πρόσβασης**

- Το blade ενοποίησης εσωτερικής εγκατάστασης εμφανίζεται μόνο σε υβριδικά περιβάλλοντα, που σημαίνει ότι χρησιμοποιείτε την επαναφορά κωδικού πρόσβασης για να χειριστείτε τους κωδικούς πρόσβασης των χρηστών εσωτερικής εγκατάστασης.
- Αυτή η λάμα δεν είναι αυτή, εάν:
    - Δεν χρησιμοποιείτε την writeback κωδικού πρόσβασης
    - Υπάρχει πρόβλημα με την εγκατάσταση/συνδεσιμότητα της writeback κωδικού πρόσβασης
    - Υπάρχει πρόβλημα με την εγκατάσταση/συνδεσιμότητα του Azure AD Connect
    - Για περισσότερα βήματα αντιμετώπισης προβλημάτων με την writeback κωδικού πρόσβασης, ανατρέξτε στην ενότητα "Αντιμετώπιση προβλημάτων με την [writeback κωδικού πρόσβασης"](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Δεν ξέρω πώς να επαναφέρω τον κωδικό πρόσβασης ενός χρήστη**

1. Πραγματοποιήστε είσοδο στην πύλη Azure ως κατάλληλος διαχειριστής.
1. Μεταβείτε στη σελίδα "Χρήστες και ομάδες" και επιλέξτε "Όλοι **οι χρήστες".**
1. Επιλέξτε ένα χρήστη από τη λίστα.
1. Για τον επιλεγμένο χρήστη, επιλέξτε **"Επισκόπηση" και,** στη συνέχεια, στη γραμμή εντολών, κάντε κλικ στην επιλογή **"Επαναφορά κωδικού πρόσβασης".**
1. Ακολουθήστε τις οδηγίες που εμφανίζονται στην οθόνη.
    - Μόνο οι επαναρυθμιώσεις που εκτελούνται μέσω της writeback κωδικού πρόσβασης υποστήριξης της πύλης Azure.

**Έχω επαναφέρει τον κωδικό πρόσβασης ενός χρήστη εσωτερικής εγκατάστασης από την πύλη διαχείρισης του Office 365 ή την εφαρμογή του Office 365 για κινητές συσκευές, αλλά ο χρήστης εξακολουθεί να μην μπορεί να κάνει είσοδο**

Η Writeback κωδικού πρόσβασης δεν υποστηρίζεται σε αυτήν την πύλη. Επαναφορά του κωδικού πρόσβασης του χρήστη ξανά στην πύλη Azure - portal.azure.com

