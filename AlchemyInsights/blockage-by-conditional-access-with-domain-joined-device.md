---
title: Έχω αποκλειστεί από την Πρόσβαση υπό όρους με μια συσκευή που είναι συνδεδεμένος με τομέα
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/20/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9834"
- "9003257"
ms.openlocfilehash: 052311ffe71bcb65de2b5c2a964932b1fb99c373
ms.sourcegitcommit: c34ba92e19419dcb2d251b8a1afe4d180a939617
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/20/2021
ms.locfileid: "51036697"
---
# <a name="im-getting-blocked-by-conditional-access-with-domain-joined-device"></a>Έχω αποκλειστεί από την Πρόσβαση υπό όρους με μια συσκευή που είναι συνδεδεμένος με τομέα

**Εργαλεία που συνιστώνται ιδιαίτερα**

[Εργαλείο αντιμετώπισης προβλημάτων εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/dsregtool/dsregtool/) - Το εργαλείο που σας βοηθά να αντιμετωπίσετε τα πιο συνηθισμένα προβλήματα εγγραφής συσκευής.

[Δοκιμή δέσμης ενεργειών συνδεσιμότητας εγγραφής συσκευής](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) - Η δέσμη ενεργειών που σας βοηθά να εξασφαλίζετε ότι μια συσκευή μπορεί να αποκτήσει πρόσβαση στα τελικά σημεία καταχώρησης συσκευής κάτω από το λογαριασμό συστήματος.

[Δέσμη ενεργειών εκκαθάρισης συσκευής Azure AD](https://github.com/mzmaili/AzureADDeviceCleanup) - Η δέσμη ενεργειών που σας επιτρέπει να αναζητήσετε και να διαχειριστείτε μη ορθές συσκευές στο περιβάλλον σας.

Ακολουθούν ορισμένοι συνηθισμένοι λόγοι για τους οποίους η πρόσβαση υπό όρους ενδέχεται να αποτυγχάνει σε μια συσκευή που έχει ενταχθεί σε έναν τομέα (Υβριδικό Azure AD).

1. **Δεν υπάρχει Azure AD PRT** στη συσκευή - Πρέπει να βεβαιωθείτε ότι η συσκευή διαθέτει Διακριτικό κύριας ανανέωσης Azure AD (PRT). Για περισσότερες πληροφορίες σχετικά με την PRT, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

Για να επαληθεύσετε εάν έχετε Azure AD PRT, μπορείτε να εκτελέσετε την εντολή στη συσκευή και να επαληθεύσετε εάν `dsregcmd/status` το "AzureAdPrt" ισούται με "ΝΑΙ".

Εάν το "AzureAdPrt" είναι "NO", ελέγξτε τα εξής:

- Εάν έχετε ένα ομόσπονδο περιβάλλον με **AD FS και** δεν είναι προσβάσιμο από τα οικιακά δίκτυα των χρηστών σας: Σε αυτή την περίπτωση, βεβαιωθείτε ότι τα τελικά σημεία "usernamemixed" είναι προσβάσιμα από το extranet. Εάν το AD FS βρίσκεται πίσω από ένα VPN, βεβαιωθείτε ότι οι χρήστες συνδέονται στο VPN και επανα-συνδέονται στη συσκευή. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains)

- **Εάν το TPM** της συσκευής είναι ελαττωματικό και, επομένως, δεν είναι δυνατός ο έλεγχος ταυτότητας της συσκευής: Ελέγξτε "tpm.msc" για να δείτε εάν η κατάσταση της TPM είναι "Ready". Εάν όχι, `dsregcmd/leave` εκτελέστε και αφήστε τη συσκευή να επανα-συμμετάσχει στο Azure AD. Στη συνέχεια, δοκιμάστε ξανά. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)

- **Χρησιμοποιείτε μια υπηρεσία παροχής ταυτότητας τρίτου κατασκευαστή, η οποία δεν υποστηρίζει WS-Trust πρωτοκόλλου.** Όπως περιγράφεται στα έγγραφά μας, οι υβριδικές συσκευές που είναι συνδεδεμένες με το Azure AD δεν μπορούν να λειτουργούν σε αυτή την περίπτωση. Συνεργαστείτε με την υπηρεσία παροχής ταυτότητας για υποστήριξη.

2. Οι χρήστες χρησιμοποιούν το πρόγραμμα περιήγησης Chrome χωρίς τους λογαριασμούς **Των Windows 10** ή την επέκταση του Office Το Chrome δεν χρησιμοποιεί αυτόματα το PRT σε συσκευές που είναι συνδεδεμένες με AAD ή σε συσκευές που είναι συνδεδεμένες με **υβριδική AAD:** Αυτό οδηγεί σε αποτυχία των πολιτικών πρόσβασης υπό όρους που βασίζονται σε συσκευή, με το μήνυμα σφάλματος "Μη καταχωρημένη συσκευή" να εμφανίζεται. Για να χρησιμοποιήσετε σωστά το πρόγραμμα περιήγησης Chrome, πρέπει να εγκαταστήσετε τους "Λογαριασμούς Windows 10" ή "Επέκταση του Office στο πρόγραμμα περιήγησης Chrome των χρηστών" μέσω SCCM ή Intune. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/conditional-access/concept-conditional-access-conditions#chrome-support)

Εάν δεν είναι δυνατή η απομακρυσμένη ώθηση της επέκτασης, ειδοποιήστε τους χρήστες να εγκαταστήσουν με μη αυτόματο τρόπο μία από τις παραπάνω επεκτάσεις για να αποκτήσουν πρόσβαση σε εφαρμογές πίσω από την πρόσβαση υπό όρους που βασίζεται σε συσκευή. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/conditional-access/require-managed-devices#prerequisites)

3. Η συσκευή συνδέθηκε σωστά με υβριδικό **Azure AD,** αλλά διαγράφηκε ή απενεργοποιήθηκε κατά λάθος, είτε λόγω αλλαγών συγχρονισμού στο Azure AD Connect είτε από την πύλη Azure: Εάν συμβεί αυτό, το αντικείμενο συσκευής δεν αναγνωρίζεται πλέον ως πλήρως συνδεδεμένο συσκευή, παρόλο που η κατάσταση "AzureAdJoined" και "PRT" εμφανίζεται ως έγκυρη στη συσκευή.

Για να διορθώσετε αυτό το πρόβλημα, `dsregcmd/leave` εκτελέστε τις συσκευές που επηρεάζονται και επιτρέψτε τους να επανασυνδετούν στο Azure AD. Για περισσότερες πληροφορίες, ανατρέξτε σε αυτό [το έγγραφο.](https://docs.microsoft.com/azure/active-directory/devices/faq#q-why-do-my-users-see-an-error-message-saying-your-organization-has-deleted-the-device-or-your-organization-has-disabled-the-device-on-their-windows-10-devices)

> [!NOTE]
> Εάν οι συσκευές σας βρίσκονται σε ενημέρωση των Windows 10, 1809, με διακομιστή μεσολάβησης VPN/cloud και δείτε προβλήματα με την κατάσταση "AzureAdPrt" ή οποιαδήποτε εφαρμογή με πρόβλημα SSO (το Outlook δεν συνδέεται στο γραμματοκιβώτιο παρόλο που είχατε PRT), βεβαιωθείτε ότι έχετε αυτή την ενημέρωση [KB4554354](https://support.microsoft.com/topic/march-30-2020-kb4554354-os-build-17763-1132-deaba49b-4b29-55b9-caee-3e2d87dd75a2) ή την αθροιστική ενημέρωση [Απριλίου KB4549949](https://support.microsoft.com/topic/april-14-2020-kb4549949-os-build-17763-1158-76d9a3af-b20b-8996-bd4d-7b50c505fda6) για να αποτρέψετε αποτυχίες PRT σε αυτούς τους υπολογιστές.

















