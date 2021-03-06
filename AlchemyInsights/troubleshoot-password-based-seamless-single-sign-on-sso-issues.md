---
title: Αντιμετώπιση προβλημάτων απρόσκοπτης σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9374"
ms.openlocfilehash: 4a9163f199a505df9b2de4f02b7c37a5f5677022
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714768"
---
# <a name="troubleshoot-password-based-seamless-single-sign-on-sso-issues"></a>Αντιμετώπιση προβλημάτων απρόσκοπτης σύνδεσης (SSO) που βασίζονται σε κωδικό πρόσβασης

Για να μάθετε τα βασικά στοιχεία της SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα ["Έλεγχος ταυτότητας βάσει κωδικού πρόσβασης" με το Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/fundamentals/auth-password-based-sso)

**Ρύθμιση παραμέτρων SSO βάσει κωδικού πρόσβασης**

1. [Ρύθμιση παραμέτρων της μεμονωμένης σύνδεσης που βασίζεται σε](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications) κωδικό πρόσβασης - Αυτό το άρθρο περιγράφει πιο αναλυτικά την επιλογή SSO που βασίζεται σε κωδικό πρόσβασης. Εάν η εφαρμογή που προσθέτετε απαιτεί προσαρμοσμένη ρύθμιση παραμέτρων και πρέπει να χρησιμοποιήσετε SSO που βασίζεται σε κωδικό πρόσβασης, αυτό το άρθρο είναι για εσάς.
2. [Ρυθμίστε τις παραμέτρους μίας σύνδεσης που βασίζεται σε](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting) κωδικό πρόσβασης για εφαρμογές εσωτερικής αποθήκευσης - Ο διακομιστής μεσολάβησης εφαρμογών υποστηρίζει πολλές λειτουργίες μονής σύνδεσης. Η σύνδεση που βασίζεται σε κωδικό πρόσβασης προορίζεται για εφαρμογές που χρησιμοποιούν συνδυασμό ονόματος χρήστη/κωδικού πρόσβασης για τον έλεγχο ταυτότητας. Όταν ρυθμίζετε τις παραμέτρους της σύνδεσης με κωδικό πρόσβασης για την εφαρμογή σας, οι χρήστες πρέπει να πραγματοποιήσουν είσοδο στην εφαρμογή εσωτερικής εγκατάστασης μία φορά. Μετά από αυτό, το Azure Active Directory αποθηκεύει τις πληροφορίες σύνδεσης και τις παρέχει αυτόματα στην εφαρμογή, όταν οι χρήστες σας έχουν πρόσβαση σε αυτές από απόσταση.
    - Θα πρέπει να έχετε ήδη δημοσιεύσει και δοκιμάσει την εφαρμογή σας με διακομιστή μεσολάβησης εφαρμογών. Εάν όχι, ακολουθήστε τα βήματα στη δημοσίευση εφαρμογών χρησιμοποιώντας το διακομιστή μεσολάβησης εφαρμογών [Azure AD,](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-add-on-premises-application) στη συνέχεια, συνεχίστε με τη ρύθμιση παραμέτρων SSO που βασίζεται σε κωδικό πρόσβασης για εφαρμογές on-prem.

Για την αντιμετώπιση προβλημάτων SSO που βασίζεται σε κωδικό πρόσβασης, ανατρέξτε στο θέμα "Αντιμετώπιση προβλημάτων μονής σύνδεσης βάσει κωδικού [πρόσβασης στο Azure AD"](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso)
