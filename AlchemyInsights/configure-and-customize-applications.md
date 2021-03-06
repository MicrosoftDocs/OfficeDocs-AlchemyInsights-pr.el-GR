---
title: Ρύθμιση παραμέτρων και προσαρμογή εφαρμογών
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
- "9004334"
- "7733"
ms.openlocfilehash: 30127beda85dd9824f7e3a7a4744d109e7ea874b
ms.sourcegitcommit: aeb15e206865f61ff61a1e55c407e34eaa89b6d1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/29/2021
ms.locfileid: "50063619"
---
# <a name="configure-and-customize-applications"></a>Ρύθμιση παραμέτρων και προσαρμογή εφαρμογών

**Ρύθμιση παραμέτρων εφαρμογών**

1. Γρήγορη εκκίνηση: Η επιλογή "Ρύθμιση παραμέτρων ιδιοτήτων για μια εφαρμογή" στον μισθωτή του [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) σάς δείχνει πώς μπορείτε να ρυθμίσετε ορισμένες από τις ιδιότητες για μια εφαρμογή.
2. Για να σας βοηθήσουμε να ενσωματώσετε τις εφαρμογές σας στο Azure Active Directory, έχουμε αναπτύξει μια συλλογή από [προγράμματα εκμάθησης που](https://docs.microsoft.com/azure/active-directory/saas-apps/tutorial-list) σας βοηθούν να διαμορφώσετε με τα προγράμματα εκμάθησης.
3. [Ο τρόπος με τον οποίο μπορείτε](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-config-how-to) να ρυθμίσετε τις παραμέτρους μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογής σάς βοηθά να κατανοήσετε τον τρόπο με τον οποίο μπορείτε να ρυθμίσετε τις παραμέτρους μιας εφαρμογής διακομιστή μεσολάβησης εφαρμογής μέσα στο Azure AD, για να εκθέσετε τις εφαρμογές εσωτερικής εγκατάστασης στο cloud.
4. Κάντε λήψη του [PingAccess](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-ping-access-publishing-guide#download-pingaccess-and-configure-your-application)και ρυθμίστε τις παραμέτρους της εφαρμογής σας: Ακολουθήστε τις οδηγίες στο άρθρο "Ρύθμιση παραμέτρων *PingAccess* για Azure AD" για την προστασία εφαρμογών που δημοσιεύονται με το διακομιστή μεσολάβησης εφαρμογών Microsoft Azure AD στην τοποθεσία Web "Ταυτότητα ping" και κάντε λήψη της πιο πρόσφατης έκδοσης του PingAccess.

**Σφάλματα εσφαλμένης ρύθμισης παραμέτρων εφαρμογής (AADSTS650056)**

1. Βεβαιωθείτε ότι έχετε πρόσβαση στην εφαρμογή από τη διεύθυνση είσοδος που παρέχεται από τον κάτοχο της εφαρμογής. Διαφορετικά, πραγματοποιήστε είσοδο στην εφαρμογή μέσω της κανονικής διεργασίας. Στις περισσότερες περιπτώσεις, η επίλυση του προβλήματος θα γίνει αυτόματα με φυσικό τρόπο. Εάν όχι, αυτή η δημοσίευση μπορεί να σας βοηθήσει στην αντιμετώπιση προβλημάτων και στην επίλυσή της.
2. **Εάν η εφαρμογή ανήκει στον οργανισμό σας (που** σημαίνει ότι η καταχώρηση της εφαρμογής ανήκει στον οργανισμό σας):
    - Τουλάχιστον, έχουμε προτείνει την προσθήκη ή `User.Read` `openid` την ανάθεση δικαιώματος από το Microsoft **Graph.**
    - Βεβαιωθείτε ότι συναινέσει η εφαρμογή και όλα τα δικαιώματά της. Μπορείτε να το επαληθεύσετε αυτό εξετάζοντας τη **στήλη "Κατάσταση"** της καταχώρησης εφαρμογής στα **"Δικαιώματα API".**
    - Σε ορισμένα σενάρια, η εφαρμογή μπορεί να είναι τρίτο μέρος, ωστόσο μπορεί να έχει καταχωρηθεί στην εταιρεία σας. Επιβεβαιώστε εάν αυτή η εφαρμογή αναφέρεται στις καταχωρήσεις εφαρμογών (όχι για μεγάλες επιχειρήσεις).
    - Εάν εξακολουθείτε να βλέπετε αυτό το μήνυμα σφάλματος. Στη συνέχεια, ίσως χρειαστεί να δημιουργήσετε τη διεύθυνση URL συγκατάθεσης που περιγράφεται **στο βήμα 4.**
3. **Εάν ο οργανισμός σας δεν είναι ο κάτοχος της εφαρμογής και τον χρησιμοποιεί ως εφαρμογή άλλου κατασκευαστή:**
    - Εάν είστε ο διαχειριστής global/company, θα πρέπει να δείτε την οθόνη συγκατάθεσης. Βεβαιωθείτε ότι έχετε ελέγξει το πλαίσιο ελέγχου **"Συγκατάθεση εκ μέρους του οργανισμού σας".**
    - Εάν δεν βλέπετε την οθόνη συγκατάθεσης, διαγράψτε την εφαρμογή για μεγάλες επιχειρήσεις και προσπαθήστε ξανά.
    - Εάν εξακολουθείτε να βλέπετε αυτό το μήνυμα σφάλματος. Στη συνέχεια, ίσως χρειαστεί να δημιουργήσετε τη διεύθυνση URL συγκατάθεσης που περιγράφεται **στο βήμα 4.**
4. Μη αυτόματη δημιουργία της διεύθυνσης **URL** συγκατάθεσης που θα χρησιμοποιηθεί: Εάν η εφαρμογή έχει σχεδιαστεί για πρόσβαση σε έναν συγκεκριμένο πόρο, ενδέχεται να μην μπορείτε να χρησιμοποιήσετε τα κουμπιά συγκατάθεσης από την πύλη Azure, θα πρέπει να δημιουργήσετε με μη αυτόματο τρόπο τη δική σας διεύθυνση URL συγκατάθεσης και να χρησιμοποιήσετε αυτήν τη διεύθυνση.
    - Θα πρέπει να λάβετε και το `{App-Id}` από τον κάτοχο της `{App-Uri-Id}` εφαρμογής. `{Tenant-Id}` θα είναι το αναγνωριστικό μισθωτή σας. Αυτό θα είναι ή `yourdomain.onmicrosoft.com` το αναγνωριστικό καταλόγου σας.
    - Εάν η εφαρμογή έχει πρόσβαση στον εαυτό της για τον πόρο, τότε το `{App-Id}` και θα είναι το `{App-Uri-Id}` ίδιο.
5. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Προβλήματα κατά την είσοδο σε εφαρμογές που βασίζονται σε μία σύνδεση που [βασίζεται σε SAML.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#misconfigured-application)

**Προσαρμογή εφαρμογών**

- Προσθέστε εμπορική προσαρμογή στη σελίδα σύνδεσης του [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/customize-branding) του οργανισμού σας - Χρησιμοποιήστε το λογότυπο της εταιρείας σας και προσαρμοσμένους συνδυασμούς χρωμάτων για να παρέχετε συνεπή εμφάνιση και αίσθηση στις σελίδες σύνδεσης του Azure Active Directory (Azure AD).
- [Προσθέστε το προσαρμοσμένο όνομα τομέα σας χρησιμοποιώντας την πύλη του Azure Active Directory](https://docs.microsoft.com/azure/active-directory/fundamentals/add-custom-domain) - Κάθε νέος μισθωτής του Azure AD συνοδεύεται από ένα αρχικό όνομα τομέα. Δεν μπορείτε να αλλάξετε ή να διαγράψετε το αρχικό όνομα τομέα, αλλά μπορείτε να προσθέσετε τα ονόματα της εταιρείας σας. Η προσθήκη προσαρμοσμένων ονομάτων τομέων σάς βοηθά να δημιουργήσετε ονόματα χρηστών που είναι οικεία για τους χρήστες σας.
