---
title: Ο συγχρονισμός UPN απενεργοποιήθηκε
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749514"
---
# <a name="upn-sync-disabled"></a>Ο συγχρονισμός UPN απενεργοποιήθηκε

Εάν αρχίσατε να συγχρονίζετε το Azure AD πριν από τις 30 Μαρτίου 2016, εκτελέστε το ακόλουθο cmdlet Azure AD PowerShell για να ενεργοποιήσετε τη μαλακή αντιστοίχιση UPN μόνο για τον οργανισμό σας:
  
 **MsolDirSyncFeature-δυνατότητα EnableSoftMatchOnUpn-ενεργοποίηση $True**
  
Το Soft Match UPN ενεργοποιείται αυτόματα για τους οργανισμούς που άρχισαν να συγχρονίζονται με το Azure AD στις ή μετά τις 30 Μαρτίου 2016.
  
Για να μάθετε περισσότερα σχετικά με την ενεργοποίηση του Soft Match στο UPN και σε άλλες δυνατότητες συγχρονισμού, ανατρέξτε στο θέμα [δυνατότητες υπηρεσίας συγχρονισμού του Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

