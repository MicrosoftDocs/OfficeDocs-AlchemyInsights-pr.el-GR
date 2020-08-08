---
title: Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555000"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a>Αντιμετώπιση προβλημάτων ανάπτυξης πιστοποιητικού ελέγχου ταυτότητας προγράμματος-πελάτη

Τα προφίλ πιστοποιητικών Intune NDES/SCEP και PKCS/PFX Client χρησιμοποιούνται συνήθως σε συνδυασμό με άλλους τύπους προφίλ, όπως Wifi, VPN και ηλεκτρονικό ταχυδρομείο, ώστε να επιτρέπεται στους χρήστες ο έλεγχος ταυτότητας σε εταιρικούς πόρους. Όταν αυτοί οι τύποι προφίλ συνδέονται με ένα προφίλ πιστοποιητικού προγράμματος-πελάτη εξαρτώνται από την επιτυχή ανάπτυξη αυτού του προφίλ.

Η αρχική εγκατάσταση υποδομής και η συσχετισμένη ρύθμιση παραμέτρων του προφίλ πιστοποιητικού προγράμματος-πελάτη συχνά απαιτούν αντιμετώπιση προβλημάτων. Για έναν οδηγό βήμα προς βήμα για την επιτυχή εγκατάσταση της σύνδεσης NDES και οδηγίες αντιμετώπισης προβλημάτων για την απομόνωση ζητημάτων με την ανάπτυξη πιστοποιητικού, ανατρέξτε στα θέματα: 

- [Ρύθμιση παραμέτρων υποδομής για υποστήριξη SCEP με Intune](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [Επισκόπηση για την αντιμετώπιση προβλημάτων προφίλ πιστοποιητικών SCEP με το Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

Χρησιμοποιήστε τις αναφερόμενες δέσμες ενεργειών powershell για να επαληθεύσετε τις παραμέτρους σας. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δέσμες ενεργειών επαλήθευσης σύνδεσης πιστοποιητικού Intune](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).

  
**Άλλα κοινά ζητήματα**

**Όταν προσπαθώ να εγκαταστήσω τη σύνδεση πιστοποιητικού Intune στο διακομιστή σύνδεσης NDES, λαμβάνω το μήνυμα, "Δεν είναι δυνατή η επαλήθευση του κωδικού πρόσβασης στην αίτηση πιστοποιητικού. Μπορεί να έχει ήδη χρησιμοποιηθεί. Αποκτήστε έναν νέο κωδικό πρόσβασης για να υποβάλετε με αυτήν την αίτηση."**  

Αυτό το μήνυμα σημαίνει ότι πρέπει να εκτελέσετε την εγκατάσταση σύνδεσης πιστοποιητικού ως διαχειριστής.

Σε ορισμένα περιβάλλοντα, οι διακομιστές όπου εκτελείται το πιστοποιητικό Intune πρέπει να χρησιμοποιούν ένα διακομιστή μεσολάβησης για να συνδεθούν με το Intune και έτσι η σύνδεση πιστοποιητικού πρέπει να χρησιμοποιεί διακομιστή μεσολάβησης. Σε ορισμένες περιπτώσεις, η σύνδεση NDES αγνοεί τις ρυθμισμένες ρυθμίσεις διακομιστή μεσολάβησης και ίσως χρειαστεί να ρυθμίσετε τις παραμέτρους του διακομιστή μεσολάβησης κατά την εκτέλεση στο περιβάλλον ασφαλείας του LocalSystem. 
 
Η λύση είναι να εκτελέσετε τον Internet Explorer ως SYSTEM και να ρυθμίσετε τις παραμέτρους ενός διακομιστή μεσολάβησης στον IE. Μετά από μια επανεκκίνηση της υπηρεσίας σύνδεσης Intune, η σύνδεση NDES συνδέεται με το Intune.

**Οι συσκευές χρήστη δεν λαμβάνουν πλέον πιστοποιητικά SCEP από το NDES.**

Είναι πιθανό το πιστοποιητικό ελέγχου ταυτότητας υπολογιστή-πελάτη που εκδόθηκε στο διακομιστή NDES και καθορίστηκε κατά την εγκατάσταση σύνδεσης NDES, να έχει λήξει ή να λείπει. Για να επιλύσετε: 
 
1. Καταργήστε την εγκατάσταση της σύνδεσης NDES.  
2. Χρησιμοποιήστε αυτές τις λεπτομέρειες για να ζητήσετε ένα νέο πιστοποιητικό ελέγχου ταυτότητας υπολογιστή-πελάτη ή διακομιστή: 
 
    - Όνομα θέματος: CN=εξωτερικό fqdn  
    - Εναλλακτικό όνομα θέματος (και τα δύο απαιτούνται): DNS=εξωτερικό fqdn, DNS=εσωτερικό fqdn 
 
3. Εγκαταστήστε ξανά τη σύνδεση NDES με το νέο πιστοποιητικό.