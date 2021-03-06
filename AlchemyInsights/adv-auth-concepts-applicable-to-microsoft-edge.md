---
title: Έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "9003931"
- "6986"
- "8329"
- "9004625"
ms.openlocfilehash: d469973c4f8605b00d32f6f625eb5fdd17e8f390
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398562"
---
# <a name="advanced-authentication-concepts-applicable-to-microsoft-edge"></a>Έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge

Ακολουθούν οι έννοιες ελέγχου ταυτότητας για προχωρημένους που ισχύουν για τον Microsoft Edge:

**Προληπτικός έλεγχος ταυτότητας**

Όταν ενεργοποιήσετε την πολιτική [ProactiveAuthEnabled,](https://go.microsoft.com/fwlink/?linkid=2134621) ο Microsoft Edge θα προσπαθήσει να πραγματοποιήσει προληπτικό έλεγχο ταυτότητας των χρηστών που είναι συνδεδεμένοι μέσω των υπηρεσιών της Microsoft. Σε τακτά χρονικά διαστήματα, θα χρησιμοποιεί μια ηλεκτρονική υπηρεσία για να ελέγχει για μια ενημερωμένη διακήρυξη που περιέχει τη ρύθμιση παραμέτρων που διέπει τον προληπτικό έλεγχο ταυτότητας.

Πλεονεκτήματα: Ο προληπτικός έλεγχος ταυτότητας επιτρέπει τον έλεγχο ταυτότητας σε βασικές υπηρεσίες, όπως η σελίδα "Νέα καρτέλα του Office". Επίσης, εάν το Bing χρησιμοποιείται ως μηχανισμός αναζήτησης, ο προληπτικός έλεγχος ταυτότητας βελτιώνει τις επιδόσεις της γραμμής διευθύνσεων και συμβάλλει στη δημιουργία αποτελεσμάτων αναζήτησης προσαρμοσμένων στις ανάγκες της επιχείρησής σας.

**Windows Hello CredUI για έλεγχο ταυτότητας NTLM**

Εάν η μεμονωμένη σύνδεση (SSO) δεν είναι διαθέσιμη όταν μια τοποθεσία Web προσπαθεί να συνδεθεί στο χρήστη μέσω του μηχανισμού NTLM ή Negotiate, αυτή η δυνατότητα θα επιτρέψει στο χρήστη να κάνει κοινή χρήση των διαπιστευτηρίων λειτουργικού συστήματος με την τοποθεσία Web και να ικανοποιεί την πρόκληση ελέγχου ταυτότητας χρησιμοποιώντας το περιβάλλον εργασίας χρήστη Windows Hello Cred. Αυτή η ροή είσοδου θα εμφανίζεται μόνο στα Windows 10 και μόνο για τους χρήστες που δεν επιτρέπουν SSO κατά τη διάρκεια ενός NTLM ή μιας πρόκλησης "Διαπραγματευτείτε".

**Χρήση αποθηκευμένων κωδικών πρόσβασης για αυτόματη είσοδο**

Οι χρήστες που αποθηκεύσουν κωδικούς πρόσβασης στον Microsoft Edge μπορούν να ενεργοποιήσουν την αυτόματη είσοδο σε τοποθεσίες Web όπου έχουν αποθηκεύσει διαπιστευτήρια. Οι χρήστες μπορούν να ενεργοποιήσουν ή να απενεργοποιήσουν αυτήν τη δυνατότητα edge://settings/passwords και μπορείτε να τη ρυθμίσετε στις πολιτικές διαχείρισης [κωδικών](https://go.microsoft.com/fwlink/?linkid=2134622) πρόσβασης.
