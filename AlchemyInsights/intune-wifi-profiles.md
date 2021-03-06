---
title: Προφίλ Wi-Fi Intune
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
- "1548"
- "9000076"
ms.openlocfilehash: e5e1007abadb8ddb30ca110d465131ec791e44b7
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555007"
---
# <a name="intune-wi-fi-profiles"></a>Προφίλ Wi-Fi Intune

Η επιτυχής υλοποίηση της συνδεσιμότητας Wi-Fi για υπολογιστές-πελάτες MDM εξαρτάται από ένα σωστά αναπτυγμένο προφίλ που αντικατοπτρίζει τις απαιτήσεις της εταιρικής υποδομής Wi-Fi. Για να εξετάσετε τις κατάλληλες ρυθμίσεις για τις πλατφόρμες-πελάτες που ερευνάτε, ανατρέξτε στα θέματα: 

[Προσθήκη ρυθμίσεων Wi-Fi για συσκευές που εκτελούν Android στο Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android)

[Προσθήκη ρυθμίσεων Wi-Fi για αποκλειστικές και πλήρως διαχειριζόμενες συσκευές Android Enterprise στο Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[Προσθήκη ρυθμίσεων Wi-Fi για συσκευές iOS και iPadOS στο Microsoft Intune](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[Προσθήκη ρυθμίσεων Wi-Fi για συσκευές Windows 10 και νεότερες συσκευές στο Intune](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[Εισαγωγή ρυθμίσεων Wi-Fi για συσκευές Windows στο Intune](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

**Κοινά θέματα**

**Αναπτύσσουμε ένα προφίλ Wi-Fi που εξαρτάται από ένα αναπτυγμένο πιστοποιητικό που καθορίζεται στο προφίλ Wi-Fi. Ωστόσο, τα προφίλ ρύθμισης παραμέτρων εμφανίζουν μια κατάσταση σφάλματος.**

Βεβαιωθείτε ότι η συσκευή σας έλαβε το πιστοποιητικό.

1. Στο Intune, μεταβείτε στην επιλογή **Όλες οι συσκευές** και επιλέξτε τη συσκευή > **ρύθμιση παραμέτρων συσκευής**.

2. Βεβαιωθείτε ότι όλα τα αναμενόμενα προφίλ παρατίθενται και βρίσκονται σε επιτυχημένη κατάσταση.

3. Για ένα προφίλ Android, αν έχετε ενδιάμεσα πιστοποιητικά στην αλυσίδα πιστοποιητικών, βεβαιωθείτε ότι έχουν αναπτυχθεί σε συσκευές Android.

    Για να ελέγξετε την κατάσταση του πιστοποιητικού, μεταβείτε στην ενότητα Προφίλ **ρύθμισης παραμέτρων συσκευής**  >  **Profiles**  >  **Με ενδιάμεσες**  >  **ιδιότητες**  >  **αρχής έκδοσης πιστοποιητικών Android Αξιόπιστο πιστοποιητικό**.

Εάν εξακολουθείτε να βλέπετε σφάλματα, εξετάστε τις διαδικασίες και τις ενότητες αντιμετώπισης προβλημάτων. Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Επισκόπηση για την αντιμετώπιση προβλημάτων προφίλ πιστοποιητικών SCEP με το Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).

**Έχω αναπτύξει ένα προφίλ Wi-Fi σε μια συσκευή. Το Intune δείχνει ότι ήταν επιτυχής, αλλά η συσκευή δεν συνδέεται με το Wi-Fi.**

Μια επιτυχημένη κατάσταση σημαίνει ότι το Intune έχει αναπτύξει με επιτυχία το προφίλ όπως έχει ρυθμιστεί. Ωστόσο, αυτές οι ρυθμίσεις παραμέτρων ενδέχεται να μην συμφωνούν με τις απαιτήσεις του δικτύου ή/και του ελέγχου ταυτότητας. Για περισσότερες λεπτομέρειες σχετικά με την επιχειρημένη σύνδεση, ανατρέξτε στα αρχεία καταγραφής στην υποδομή και την υπηρεσία ελέγχου ταυτότητας (στον ελεγκτή σημείου πρόσβασης Wi-Fi και στο διακομιστή NPS/Radius). Ίσως χρειαστεί να συνεργαστείτε με την ομάδα υποδομής δικτύου ή με τον τρίτο προμηθευτή Wi-Fi, για να συγκεντρώσετε και να αναθεωρήσετε αρχεία καταγραφής.