---
title: 2681 Attack Simulator στο Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545726"
---
# <a name="attack-simulator-in-microsoft-365"></a>Ο Εξομοιωτής επίθεσης Microsoft 365

- Σας λείπει ο Εξομοιωτής επίθεσης; Το Attack Defender **απαιτεί τον Microsoft Defender Office 365 πρόγραμμα 2** ή Office 365 για μεγάλες επιχειρήσεις **E5.** Το Attack Simulator **δεν** περιλαμβάνεται στο Microsoft Defender για Office 365 Πρόγραμμα 1, Office 365 για μεγάλες επιχειρήσεις E3 ή σε Εφαρμογές Microsoft 365 για επιχειρήσεις συνδρομές.

- Ο λογαριασμός που χρησιμοποιείτε για την εκκίνηση προσομοιωμενών επιθέσεων απαιτεί δικαιώματα καθολικού διαχειριστή ή διαχειριστή ασφαλείας και έλεγχο ταυτότητας πολλών παραγόντων (MFA). Για περισσότερες πληροφορίες σχετικά με τις απαιτήσεις του Attack Simulator, ανατρέξτε [σε αυτό το θέμα.](/microsoft-365/security/office-365-security/attack-simulator)

- Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με τις **προσομοιώσεις επίθεσης του Brute Force Password:**

  - Εάν ο λογαριασμός προορισμού έχει ενεργοποιήσει το MFA και ο κωδικός πρόσβασης έχει γίνει σωστή μαντέψει, ο λογαριασμός δεν θα εμφανίζεται ως παραβιαστείς (ο δεύτερος παράγοντας ελέγχου ταυτότητας θα είναι ημιτελής).

  - Το αρχείο κωδικού πρόσβασης δεν μπορεί να είναι μεγαλύτερο από 10 MB. Χρησιμοποιήστε έναν κωδικό πρόσβασης ανά γραμμή και συμπεριλάβετε μια κενή γραμμή (επαναφορά) μετά τον τελευταίο κωδικό πρόσβασης στη λίστα.

- Σημαντικά πράγματα που πρέπει να γνωρίζετε σχετικά με την **επισύναψη προσομοιώσεων ηλεκτρονικού "ψαρέματος** με δόρυ":

  - Από τη σχεδίαση, δεν μπορείτε να δώσετε μια προσαρμοσμένη τιμή για τη διεύθυνση URL του διακομιστή **σύνδεσης ηλεκτρονικού "ψαρέματος".**

  - Εάν ένας παραλήπτης χρησιμοποιεί το πρόσθετο ["Ενεργοποίηση](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) μηνύματος αναφοράς" για να αναφέρει το μήνυμα ως ηλεκτρονικό "ψάρεμα", ενδέχεται να μην λαμβάνετε ειδοποιήσεις για το μήνυμα (επειδή πρόκειται για προσομοιωμένη επίθεση).

- Αναφορές: Μετά την ολοκλήρωση της προσομοιωμένης επίθεσης, μπορείτε να κάνετε κλικ **στην επιλογή "Λεπτομέρειες επίθεσης"** για να δείτε την αναφορά.

- Για λεπτομερείς οδηγίες και νέες δυνατότητες στον Εξομοιωτή επίθεσης, ανατρέξτε στο θέμα ["Προσομοίωση επίθεσης" Microsoft 365.](/microsoft-365/security/office-365-security/attack-simulator)
