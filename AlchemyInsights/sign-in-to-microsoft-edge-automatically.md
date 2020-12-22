---
title: Αυτόματη είσοδος στο Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677763"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Αυτόματη είσοδος στο Microsoft Edge

Το Microsoft Edge χρησιμοποιεί τον προεπιλεγμένο λογαριασμό του λειτουργικού συστήματος για την αυτόματη είσοδο ενός χρήστη σύμφωνα με τον τρόπο ρύθμισης των παραμέτρων της συσκευής του χρήστη. 

Τα σενάρια κάθε τύπου ρύθμισης παραμέτρων συσκευής και η εξαρτώμενη διαδικασία εισόδου χρήστη περιγράφονται παρακάτω:

1. **Η συσκευή είναι υβριδική/AAD-J**: αυτή η επιλογή είναι διαθέσιμη στα Windows 10, τα παράθυρα κάτω επιπέδου και τις αντίστοιχες εκδόσεις διακομιστή. Οι χρήστες εγγράφονται αυτόματα με τους λογαριασμούς τους Azure Active Directory (AD).
2. **Η συσκευή είναι συνδεδεμένος με τομέα**: αυτή η επιλογή είναι διαθέσιμη στα Windows 10, τα παράθυρα κάτω επιπέδου και τις αντίστοιχες εκδόσεις διακομιστή. Από προεπιλογή, οι χρήστες με λογαριασμούς τομέα δεν έχουν εισέλθει αυτόματα. για να ενεργοποιήσετε την αυτόματη είσοδο για αυτούς, χρησιμοποιήστε την πολιτική **ConfigureOnPremisesAccountAutoSignIn** . Για να ενεργοποιήσετε την αυτόματη είσοδο για τους χρήστες με λογαριασμούς Azure AD, εξετάστε το ενδεχόμενο υβριδική συμμετοχή στις συσκευές τους.
3. **Ο προεπιλεγμένος λογαριασμός του λειτουργικού συστήματος είναι ένας λογαριασμός Microsoft**: αυτή η επιλογή είναι διαθέσιμη σε Windows 10 RS3 (έκδοση 1709, δομή 10.0.16299) και νεότερες εκδόσεις. Το σενάριο είναι απίθανο να προκύψει σε εταιρικές συσκευές. Ωστόσο, εάν ο προεπιλεγμένος λογαριασμός του λειτουργικού συστήματος είναι λογαριασμός Microsoft, τότε το Microsoft Edge θα εισέλθει αυτόματα στο χρήστη με το λογαριασμό Microsoft.
 
 