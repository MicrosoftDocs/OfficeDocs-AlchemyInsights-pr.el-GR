---
title: Προβλήματα με τη χρήση της κονσόλας διαχείρισης Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555039"
---
# <a name="problems-using-the-intune-admin-console"></a>Προβλήματα με τη χρήση της κονσόλας διαχείρισης Intune

**"Δεν επιτρέπεται η πρόσβαση" κατά την περιήγηση στην πύλη διαχείρισης Intune.**

- Εάν είστε μέλος ενός προσαρμοσμένου ρόλου Intune, βεβαιωθείτε ότι έχει εκχωρηθεί στο λογαριασμό σας μια άδεια χρήσης Intune ή Enterprise Mobility Suite (EMS).
- Εάν χρησιμοποιείτε τη Διαχείριση ρύθμισης παραμέτρων για τη διαχείριση συσκευών, βεβαιωθείτε ότι δεν είστε μέρος της συλλογής χρηστών Intune για το MDM της Διαχείρισης ρύθμισης παραμέτρων.
- Βεβαιωθείτε ότι σας έχουν εκχωρηθεί τα κατάλληλα δικαιώματα ελέγχου διαχείρισης που βασίζονται σε ρόλους (RBAC) στη λεπίδα ρόλων Intune.
- Βεβαιωθείτε ότι η ομάδα που χρησιμοποιείται δεν είναι λίστα διανομής. Το Intune στην πύλη Azure υποστηρίζει μόνο λογαριασμούς χρηστών που ανήκουν σε ομάδες ασφαλείας της υπηρεσίας καταλόγου Active Directory Azure. Εξετάστε τις ομάδες σας στην πύλη Azure > ομάδες **Intune**  >  **Groups**ή στην πύλη Azure > υπηρεσία καταλόγου Azure **Active Directory**.

**Ο χρήστης έχει πάρα πολλά δικαιώματα για το ρόλο Intune που έχει εκχωρηθεί**

Συμβουλέψτε το χρήστη να μεταβεί **στους ρόλους Intune**  >  **Intune**  >  **Τα δικαιώματά μου**  >  **Εξαγωγή** για να αναθεωρήσετε τα εκχωρημένα δικαιώματα.

**Πρόσθεσα μια ομάδα εμβέλειας σε ένα ρόλο, αλλά οι χρήστες σε αυτόν το ρόλο εξακολουθούν να βλέπουν άλλους χρήστες ή συσκευές.**

Οι ομάδες εμβέλειας δεν φιλτράρουν χρήστες ή συσκευές. Ομάδες εμβέλειας:

- Περιορίστε σε ποιους χρήστες μπορούν να εκχωρήσουν πολιτικές ή εφαρμογές.
- Να επιτρέπεται μόνο σε συγκεκριμένους χρήστες να εκτελούν απομακρυσμένες εργασίες σε συσκευές.

Για περισσότερες πληροφορίες σχετικά με τις ομάδες εμβέλειας, ανατρέξτε στο θέμα [Έλεγχος πρόσβασης βάσει ρόλων (RBAC) με το Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Πρόσθεσα ένα χρήστη σε ένα ρόλο Intune, αλλά εξακολουθούν να έχουν πλήρη πρόσβαση στην κονσόλα admin Intune.**

Μεταβείτε στο Intune > **χρήστες** στην πύλη Azure και βεβαιωθείτε ότι ο χρήστης δεν έχει αντιστοιχιστεί σε κανέναν από τους ακόλουθους ρόλους στην πύλη Azure:

- Καθολικός διαχειριστής
- Διαχειριστής υπηρεσίας Intune
- Διαχειριστής του SharePoint

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Έλεγχος πρόσβασης βάσει ρόλων (RBAC) με το Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).

**Θέματα πρόσβασης**

Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Δεν μπορείτε να εισέλθετε στο Office 365, azure ή Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).