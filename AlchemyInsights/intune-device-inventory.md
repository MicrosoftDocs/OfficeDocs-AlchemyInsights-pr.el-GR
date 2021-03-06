---
title: Απογραφή συσκευής Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: 5d2be7485be8578f7fdee3216dc6f3970be67fd1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667878"
---
# <a name="intune-device-inventory"></a>Απογραφή συσκευής Intune

Η λεπίδα Devices παρέχει στον διαχειριστή πληροφορίες για τις συσκευές που βρίσκονται υπό διαχείριση στο Intune σε βάση ανά συσκευή. Οι πληροφορίες που εμφανίζονται περιλαμβάνουν: υλικό, ανακαλύφθηκαν εφαρμογές, κατάσταση συμμόρφωσης συσκευής και κατάσταση ρύθμισης παραμέτρων συσκευής.

Τα δεδομένα απογραφής για το υλικό και τις ανακαλυφθείσες εφαρμογές συλλέγονται σε έναν κύκλο επτά ημερών. Οι εφαρμογές και τα συγκεκριμένα στοιχεία του υλικού που αναφέρθηκαν διαφέρουν ανάλογα με το λειτουργικό σύστημα της συσκευής και εάν η συσκευή είναι προσωπική ή εταιρική.

Για περισσότερες πληροφορίες, ανατρέξτε [στο θέμα ανατρέξτε στο θέμα λεπτομέρειες συσκευής στο Intune](https://docs.microsoft.com/intune/device-inventory).

**ΣΥΝΗΘΕΙΣ ΕΡΩΤΉΣΕΙΣ**

Ε: δεν λαμβάνω μια πλήρη λίστα απογραφής των εφαρμογών που υπάρχουν σε συσκευές Windows που έχουν εγγραφεί στο Intune. Γιατί όχι?

Α: αυτήν τη στιγμή, μόνο οι σύγχρονες εφαρμογές παρατίθενται για υπολογιστές με Windows 10 που προσδιορίζονται ως εταιρικές συσκευές. Το Intune δεν συλλέγει πληροφορίες σχετικά με τις εφαρμογές Win32 που είναι εγκατεστημένες σε αυτές τις συσκευές.

Ε: Γιατί οι αριθμοί τηλεφώνου δεν συλλέγονται από όλες τις συσκευές;

Α: τα τηλέφωνα που κατηγοριοποιούνται ως εταιρικές συσκευές στο Intune δεν προσδιορίζονται με τον πλήρη αριθμό τηλεφώνου τους όταν, για παράδειγμα, εκτελείτε μια αναφορά απογραφής κινητής συσκευής. Οι αριθμοί τηλεφώνου "μεταφορά σε εσάς" είναι πάντα μερικώς καλυμμένοι με αστερίσκους (* * * *) και εμφανίζουν μόνο τα τελευταία τέσσερα ψηφία.