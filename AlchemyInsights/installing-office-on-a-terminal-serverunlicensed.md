---
title: Εγκατάσταση του Office σε διακομιστή τερματικού-χωρίς άδεια χρήσης
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663117"
---
# <a name="installing-office-on-a-terminal-server"></a>Εγκατάσταση του Office σε διακομιστή τερματικού

Για την ανάπτυξη εφαρμογών του Microsoft 365 για επιχειρήσεις σε Windows Server με χρήση υπηρεσιών απομακρυσμένης επιφάνειας εργασίας (RDS), παλαιότερα επώνυμων υπηρεσιών Terminal Services:
  
- Πρέπει να έχετε μια συνδρομή Microsoft 365 που περιλαμβάνει εφαρμογές του Microsoft 365 για επιχειρήσεις, όπως το Office 365 Enterprise E3 ή το Enterprise E5. Οι εφαρμογές Microsoft 365 για επιχειρήσεις και Microsoft 365 για προγράμματα Premium για επιχειρήσεις δεν περιλαμβάνουν εφαρμογές του Microsoft 365 για επιχειρήσεις.

- Πρέπει να ενεργοποιήσετε την [Ενεργοποίηση του κοινόχρηστου υπολογιστή](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Εάν θέλετε να εγκαταστήσετε τις εφαρμογές του Microsoft 365 για επιχειρήσεις σε RDS από το κέντρο διαχείρισης του Microsoft 365, το ***οποίο χρησιμοποιεί τις προεπιλεγμένες ρυθμίσεις εγκατάστασης***, χρησιμοποιήστε τα παρακάτω βήματα.

> [!TIP]
> Μπορείτε επίσης να κάνετε λήψη και να εκτελέσετε τον [Βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SaRA_OfficeSCA_M365Portal) για να εγκαταστήσετε τις εφαρμογές Microsoft 365 για επιχειρήσεις σε λειτουργία ενεργοποίησης κοινόχρηστων υπολογιστών.
  
1. Επιλέξτε τη συνδρομή Microsoft 365 που έχετε. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Εάν είναι απαραίτητο, μεταβείτε σε μια διαφορετική συνδρομή του Microsoft 365. [Μάθετε πώς](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Εάν το Office είναι ήδη εγκατεστημένο στο διακομιστή RDS χρησιμοποιώντας οποιεσδήποτε άλλες συνδρομές του Microsoft 365, καταργήστε την εγκατάστασή του. Για παράδειγμα, μεταβαίνοντας στον πίνακα ελέγχου, \> καταργήστε την εγκατάσταση ενός προγράμματος. Καταργήστε την εγκατάσταση χρησιμοποιώντας [το βοηθό υποστήριξης και αποκατάστασης της Microsoft](https://aka.ms/SARA-OfficeUninstall-Alchemy) , εάν αντιμετωπίζετε προβλήματα.

4. Στο διακομιστή RDS, πραγματοποιήστε είσοδο στο κέντρο διαχείρισης του Microsoft 365 με το λογαριασμό διαχειριστή σας και [Εγκαταστήστε τις εφαρμογές microsoft 365 για επιχειρήσεις](https://portal.office.com/OLS/MySoftware.aspx).

5. Μετά την εγκατάσταση του Office, ***Μην ανοίγετε ή εισέρχεστε*** σε οποιαδήποτε εφαρμογή του Office.

6. Στο διακομιστή RDS, ενεργοποιήστε την ενεργοποίηση του κοινόχρηστου υπολογιστή, επεξεργαζόμενοι το μητρώο ακολουθώντας τα παρακάτω βήματα:

1. Κάντε δεξί κλικ στο κουμπί των Windows στην κάτω αριστερή γωνία της οθόνης σας και επιλέξτε εκτέλεση. Στο πλαίσιο Άνοιγμα, πληκτρολογήστε **regedit**και, στη συνέχεια, επιλέξτε OK.

2. Επιλέξτε Ναι όταν σας ζητηθεί να επιτρέψετε στον επεξεργαστή μητρώου να κάνει αλλαγές στη συσκευή σας.

3. Στον επεξεργαστή μητρώου, προσθέστε μια τιμή συμβολοσειράς του **SharedComputerLicensing** με μια ρύθμιση 1 στην περιοχή HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. Στο διακομιστή RDS, ***Πραγματοποιήστε είσοδο ως τελικός χρήστης*** και [Επαληθεύστε ότι η ενεργοποίηση του κοινόχρηστου υπολογιστή είναι ενεργοποιημένη για τις εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Για περισσότερες λεπτομέρειες σχετικά με τις προϋποθέσεις, τις οδηγίες εγκατάστασης και τις οδηγίες σχετικά με τις προσαρμοσμένες εγκαταστάσεις χρησιμοποιώντας το εργαλείο ανάπτυξης του Office, ανατρέξτε στο θέμα [ανάπτυξη εφαρμογών Microsoft 365 για επιχειρήσεις με τη χρήση υπηρεσιών απομακρυσμένης επιφάνειας εργασίας](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Για να διορθώσετε σφάλματα που σχετίζονται με την ενεργοποίηση του κοινόχρηστου υπολογιστή, ανατρέξτε στο [θέμα Αντιμετώπιση προβλημάτων με την ενεργοποίηση του κοινόχρηστου υπολογιστή για τις εφαρμογές Microsoft 365 για επιχειρήσεις](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  