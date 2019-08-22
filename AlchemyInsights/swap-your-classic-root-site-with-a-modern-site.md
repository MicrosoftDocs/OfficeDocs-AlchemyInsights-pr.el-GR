---
title: Εναλλαγή σας κλασικό ριζική τοποθεσία με μια σύγχρονη τοποθεσία
ms.author: efrene
author: efrene
ms.date: 8/6/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000687"
- "2579"
ms.openlocfilehash: 0f6f962314d9099bd21c281a23ad2e95742da4a8
ms.sourcegitcommit: 631e527967f4d641bc9227642ffe38967ae87a00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/09/2019
ms.locfileid: "36270744"
---
# <a name="swap-your-classic-root-site-with-a-modern-site"></a>Εναλλαγή σας κλασικό ριζική τοποθεσία με μια σύγχρονη τοποθεσία

Εάν το περιβάλλον σας έχει οριστεί πριν από Απριλίου 2019, μπορείτε να αλλάξετε τη βασική τοποθεσία σε μια σύγχρονη τοποθεσία χρησιμοποιώντας Microsoft PowerShell:

- Εάν έχετε μια διαφορετική τοποθεσία που θέλετε να χρησιμοποιήσετε ως τη βασική τοποθεσία, μπορείτε να αντικαταστήσετε την τοποθεσία (μετάθεσης) στη ρίζα με αυτό. 
    - Χρησιμοποιήστε [Invoke SPSiteSwap](https://docs.microsoft.com/powershell/module/sharepoint-online/invoke-spositeswap?view=sharepoint-ps) να αλλάξετε τη θέση μιας τοποθεσίας με άλλη τοποθεσία κατά την αρχειοθέτηση στην αρχική τοποθεσία. Διαθέσιμο για τοποθεσία ομάδας (που δεν είναι συνδεδεμένοι σε μια ομάδα) και τοποθεσία επικοινωνίας. 

- Πρόσθετες δυνατότητες θα εμφανιστούν σύντομα που θα σας επιτρέψει να διατηρήσετε χρησιμοποιώντας το περιεχόμενο της τοποθεσίας, αλλά να μετατρέψετε την υπάρχουσα τοποθεσία σε μια τοποθεσία επικοινωνίας. 
>[!Important]
>Αυτές οι δυνατότητες θα γίνει επαναφορά σταδιακά. Συνεχίσει να ελέγχει το Κέντρο μηνυμάτων του Office 365 για ενημερωμένες εκδόσεις. 

## <a name="known-issues-with-swapping-sites"></a>Γνωστά ζητήματα σχετικά με την ανταλλαγή τοποθεσίες

- Η τοποθεσία προορισμού μπορεί να επιστρέψει ένα σφάλμα "δεν βρέθηκε" (HTTP 404) για ένα μικρό χρονικό διάστημα.
- Το περιεχόμενο θα πρέπει να γίνει νέα προσπάθεια ανίχνευσης για να ενημερώσετε το ευρετήριο αναζήτησης. Υπάρχει κάποια μη αυτόματη απαιτείται - αυτό θα γίνει αυτόματα.
- Οτιδήποτε εξαρτάται από "στατική" Συνδέσεις (όπως αρχεία συγχρονισμού αρχείων και το OneNote) θα πρέπει να διορθωθούν με μη αυτόματο τρόπο.
- Εάν η τοποθεσία προέλευσης ήταν μια τοποθεσία εταιρικά νέα, ενημερώστε τη διεύθυνση URL.Λάβετε μια λίστα όλων των τοποθεσιών εταιρικά νέα.
- Τοποθεσίες του Project Server ενδέχεται να πρέπει να είναι επικυρωμένες ώστε να διασφαλίζεται ότι έχουν συσχετιστεί ακόμα σωστά.




