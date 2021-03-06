---
title: Θέλετε να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ως ασφαλή;
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 57d1e2d696a8be42b5f868f021d829bf019349bf
ms.sourcegitcommit: 3994cece80410371330b39f7b79b1b1c1bfcf648
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/08/2021
ms.locfileid: "52286680"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Θέλετε να επισημάνετε έναν τομέα ή έναν αποστολέα ηλεκτρονικού ταχυδρομείου ως ασφαλή;

- Η χρήση **ασφαλών λιστών αποστολέων δεν συνιστάται,** καθώς ανοίγει τον οργανισμό σας σε επιθέσεις ανεπιθύμητης αλληλογραφίας, ηλεκτρονικού "ψαρέματος" και πλαστογράφησης.
- Ωστόσο, εάν υπάρχει επιχειρηματική απαίτηση, συνιστάται να χρησιμοποιήσετε **τους** Κανόνες **[αλληλογραφίας Flow για](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** αυτό. Οι οδηγίες μας διασφαλίζουν τον έλεγχο ταυτότητας αποστολέα (επαληθεύει ότι ο τομέας αποστολής δεν πλαστογραφήθηκε). **Σημείωση:** Δεν συνιστάται η διαχείριση ψευδών θετικών με τη χρήση λιστών ασφαλών αποστολέων, επειδή οι εξαιρέσεις στο φιλτράρισμα ανεπιθύμητης αλληλογραφίας μπορούν να ανοίξουν τον οργανισμό σας σε επιθέσεις ασφαλείας. Εάν οι χρήστες σας λαμβάνουν μηνύματα που έχουν επισημανθεί εσφαλμένα ως ανεπιθύμητη αλληλογραφία ή ανεπιθύμητη αλληλογραφία, **[αναφέρετε μηνύματα και αρχεία στη Microsoft.](https://protection.office.com/reportsubmission)**
- Οι ασφαλείς αποστολείς στο Outlook, τη λίστα επιτρεπόμενων αποστολέων  ή τη λίστα επιτρεπόμενων τομέων στις πολιτικές καταπολέμησης της ανεπιθύμητης αλληλογραφίας θα πρέπει να αποφεύγονται, επειδή οι αποστολείς παρακάμπτουν όλα τα μηνύματα ανεπιθύμητης αλληλογραφίας, την πλαστογράφηση και την προστασία ηλεκτρονικού "ψαρέματος" και τον έλεγχο ταυτότητας αποστολέα (SPF, DKIM, DMARC). Αυτή η μέθοδος χρησιμοποιείται καλύτερα μόνο για προσωρινούς ελέγχους.
- Η επικύρωση ότι μια συγκεκριμένη αξιολόγηση Antispam που παρακάμπτεται μέσω ηλεκτρονικού ταχυδρομείου μπορεί να γίνει ελέγχοντας την κεφαλίδα μηνύματος "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), ανατρέξτε στο θέμα Κεφαλίδες μηνυμάτων **[ανεπιθύμητης αλληλογραφίας.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Επειδή η Microsoft θέλει να διατηρήσει ασφαλείς τους πελάτες της [από προεπιλογή,](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)ορισμένες παρακάμψεις μισθωτή δεν εφαρμόζονται για λογισμικό κακόβουλης λειτουργίας και ηλεκτρονικό "ψάρεμα" υψηλής εμπιστοσύνης. Αυτές οι παρακάμψεις περιλαμβάνουν: o Λίστες επιτρεπόμενων αποστολέων ή επιτρεπόμενες λίστες τομέων (πολιτικές καταπολέμησης της ανεπιθύμητης αλληλογραφίας) o Outlook Λίστα ασφαλών αποστολέων o Λίστα επιτρεπόμενων διευθύνσεων IP (φιλτράρισμα σύνδεσης) 
- Η μόνη παράκαμψη που επιτρέπει την παράκαμψη του φιλτραρίσματος του μηνύματος ηλεκτρονικού "ψαρέματος" υψηλής εμπιστοσύνης είναι Exchange κανόνες ροής αλληλογραφίας (γνωστοί και ως κανόνες μεταφοράς). Για να χρησιμοποιήσετε κανόνες ροής αλληλογραφίας για να παρακάμψετε το φιλτράρισμα, ανατρέξτε στο θέμα Χρήση κανόνων ροής αλληλογραφίας για τον ορισμό του επιπέδου εμπιστοσύνης ανεπιθύμητης **[αλληλογραφίας (SCL) στα μηνύματα.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**