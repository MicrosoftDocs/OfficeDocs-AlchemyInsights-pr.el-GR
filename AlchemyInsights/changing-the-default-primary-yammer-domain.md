---
title: Αλλαγή του προεπιλεγμένου τομέα Yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002662"
- "5162"
ms.openlocfilehash: 099feb5c58a2b1068a2ec501ff966c6ac73d804d
ms.sourcegitcommit: 87aa36e3ff4835efb120a320c5169bfa77199ec4
ms.translationtype: HT
ms.contentlocale: el-GR
ms.lasthandoff: 05/01/2020
ms.locfileid: "43991195"
---
# <a name="changing-the-defaultprimary-yammer-domain"></a>Αλλαγή του προεπιλεγμένου/κύριου τομέα Yammer

Η διεύθυνση URL του Yammer περιέχει το τρέχον όνομα του κύριου τομέα για το δίκτυο Yammer. Αυτό το όνομα τομέα ενδέχεται να μην συμφωνεί με το όνομα του κύριου τομέα που έχει οριστεί στο Office 365 ή στο Azure AD. Υπάρχουν διαφορές στη συμπεριφορά με βάση τον αριθμό των προσαρμοσμένων τομέων που έχουν προστεθεί στο μισθωτή και το εάν το Yammer βρίσκεται σε υποστηριζόμενη ρύθμιση παραμέτρων (1 μισθωτής: 1 δίκτυο, ή 1:1). Διατίθεται τεκμηρίωση σχετικά με τους [τομείς Yammer και το Office 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/manage-yammer-domains).

Ο πιο συνηθισμένος λόγος για τον οποίο βλέπετε έναν εσφαλμένο τομέα είναι ότι υπάρχουν πολλά δίκτυα Yammer και πρέπει να ενοποιηθούν. [Η ενοποίηση σε ένα ενιαίο δίκτυο](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks) χρησιμοποιώντας το εργαλείο μετεγκατάστασης δικτύου είναι το πρώτο σημαντικό βήμα. Ολοκληρώστε το πριν επιχειρήσετε να ορίσετε τον κύριο τομέα σας.

**Δεν υπάρχουν προσαρμοσμένοι τομείς**

Για τους νέους μισθωτές, ο προεπιλεγμένος τομέας (π.χ. fabrikam.onmicrosoft.com) από το μισθωτή θα χρησιμοποιηθεί για το Yammer. Ο κύριος τομέας ορίζεται σε yammer.com/fabrikam.onmicrosoft.com.

**Ενιαίος προσαρμοσμένος τομέας**

Το Yammer θα επιλέξει αυτόματα τον προσαρμοσμένο τομέα (π.χ. fabrikam.com) από το μισθωτή ως τον κύριο τομέα στο Yammer. Ορίζεται σε yammer.com/fabrikam.com. Αυτή η αλλαγή γίνεται από την υπηρεσία συγχρονισμού τομέα και μπορεί να χρειαστούν έως και 24 ώρες για να τεθεί σε ισχύ.

**Πολλοί προσαρμοσμένοι τομείς**

Το Yammer μπορεί να έχει έναν κύριο τομέα που είναι διαφορετικός από τον προεπιλεγμένο τομέα μισθωτή. Δεδομένου ότι υπάρχουν πολλοί προσαρμοσμένοι τομείς, το Yammer δεν επιχειρεί να εκτιμήσει τον σωστό τομέα από αυτούς που είναι διαθέσιμοι. Πρέπει να ανοίξετε μια υπόθεση υποστήριξης για να ζητήσετε να αλλάξει το όνομα του κύριου τομέα με τον κύριο τομέα της επιλογής σας.

**Πληροφορίες για πρόσθετους τρόπους αντιμετώπισης**

Σε ορισμένες περιπτώσεις, μπορεί κάποιοι τομείς να έχουν μετακινηθεί μεταξύ μισθωτών και η υπηρεσία συγχρονισμού τομέα δεν ήταν δυνατό να λειτουργήσει με επιτυχία. Μπορεί να αντιμετωπίσετε προβλήματα εισόδου ή άλλα προβλήματα, καθώς και έναν εσφαλμένο κύριο τομέα. Για να επιλύσετε αυτό το πρόβλημα, μπορεί να χρειαστεί να μετακινηθούν οι τομείς στο σωστό δίκτυο με τη βοήθεια της υποστήριξης της Microsoft. Αυτή η κατάσταση απαιτεί άμεση βοήθεια και μπορεί να χρειαστεί χρόνο για να επιλυθεί, ειδικά εάν υπάρχει μια πολύ μεγάλη λίστα με ονόματα τομέων. Ανοίξτε μια υπόθεση υποστήριξης για να λάβετε βοήθεια σχετικά με την επίλυση αυτών των τύπων ζητημάτων.

Ο εκπρόσωπος υποστήριξης θα ελέγξει αν οι τομείς έχουν επαληθευτεί στο μισθωτή που βρίσκεται υπό τον έλεγχό σας. Μπορεί να υποβάλει πρόσθετες ερωτήσεις επαλήθευσης σχετικά με τους τομείς σας, εάν έχουν προστεθεί στο μισθωτή σας, αλλά δεν έχουν επαληθευτεί από το DNS. Βεβαιωθείτε ότι οι τομείς έχουν επαληθευτεί από το DNS για να επιταχύνετε τη διαδικασία.