---
title: Ομοσπονδία ADFS πιστοποιητικού που λήγει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 6/8/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 6170265dac1eebe8fa1acf766d2eb8d6b0a5908b
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29662363"
---
# <a name="adfs-federation-certificate-expiring"></a><span data-ttu-id="611c1-102">Ομοσπονδία ADFS πιστοποιητικού που λήγει</span><span class="sxs-lookup"><span data-stu-id="611c1-102">ADFS Federation Certificate Expiring</span></span>

<span data-ttu-id="611c1-103">Για να επιλύσετε αυτό το ζήτημα, ακολουθήστε τα εξής βήματα:</span><span class="sxs-lookup"><span data-stu-id="611c1-103">To resolve this issue, follow these steps:</span></span>
  
1. <span data-ttu-id="611c1-p101">Εγκαταστήστε το Microsoft Azure Active Directory λειτουργική μονάδα για Windows PowerShell στον υπολογιστή (Εάν η λειτουργική μονάδα δεν είναι ήδη εγκατεστημένο). Για να γίνει αυτό, μεταβείτε στην [Διαχείριση AD Azure χρησιμοποιώντας το Windows PowerShell](https://aka.ms/aadposh).</span><span class="sxs-lookup"><span data-stu-id="611c1-p101">Install the Microsoft Azure Active Directory Module for Windows PowerShell on the computer (if the module isn't already installed). To do this, go to [Manage Azure AD using Windows PowerShell](https://aka.ms/aadposh).</span></span>
    
2. <span data-ttu-id="611c1-106">Ακολουθήστε τα βήματα του "σενάριο 1: λήξει το πιστοποιητικό υπογραφής διακριτικό AD FS" ενότητα ["Παρουσιάστηκε ένα πρόβλημα κατά την πρόσβαση στην τοποθεσία" σφάλμα από AD FS όταν μια ομόσπονδη χρήστης υπογράφει Office 365, Azure, ή Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span><span class="sxs-lookup"><span data-stu-id="611c1-106">Follow the steps in the "Scenario 1: The AD FS token-signing certificate expired" section of ["There was a problem accessing the site" error from AD FS when a federated user signs in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat).</span></span>
    
3. <span data-ttu-id="611c1-107">Ακολουθήστε τα βήματα στο [πώς μπορείτε να ενημερώσετε ή να επιδιορθώσετε τις ρυθμίσεις ομόσπονδη τομέα στο Office 365, Azure, ή Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span><span class="sxs-lookup"><span data-stu-id="611c1-107">Follow the steps in [How to update or repair the settings of a federated domain in Office 365, Azure, or Intune](https://support.microsoft.com/help/2647048/how-to-update-or-repair-the-settings-of-a-federated-domain-in-office-3).</span></span>
    
    <span data-ttu-id="611c1-108">Για να μάθετε περισσότερα σχετικά με την ανανέωση πιστοποιητικών Ομοσπονδία, ανατρέξτε στην ενότητα " [Ανανέωση πιστοποιητικών Ομοσπονδία για Office 365 και Azure υπηρεσίας καταλόγου Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)".</span><span class="sxs-lookup"><span data-stu-id="611c1-108">To learn more about renewing Federation certificates, see [Renew federation certificates for Office 365 and Azure Active Directory](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs).</span></span>
    
