---
title: Προβλήματα σύνδεσης του SharePoint Designer
ms.author: efrene
author: efrene
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f2b1b6b4-10c9-4e83-b9cb-529a0b8a3c55
ms.openlocfilehash: 1d3f6ad3128292a9dbcc46cc7da23af59a63fbb4
ms.sourcegitcommit: a285c609319ade038461e090e14a701830031825
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840551"
---
# <a name="sharepoint-designer-connection-issues"></a><span data-ttu-id="cc0d1-102">Προβλήματα σύνδεσης του SharePoint Designer</span><span class="sxs-lookup"><span data-stu-id="cc0d1-102">SharePoint Designer connection issues</span></span> 

<span data-ttu-id="cc0d1-103">Εάν το SharePoint Designer αντιμετωπίζει ζητήματα σύνδεσης σε τοποθεσίες του SharePoint, δοκιμάστε τις ακόλουθες κοινές λύσεις.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-103">If SharePoint Designer is experiencing connection issues to SharePoint sites, please try the following common solutions.</span></span>

<span data-ttu-id="cc0d1-104">Βήμα 1: Βεβαιωθείτε ότι το SharePoint Designer 2013 ενημερώνεται με [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) και [2 Αυγούστου 2016 ενημερωμένη έκδοση για το SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span><span class="sxs-lookup"><span data-stu-id="cc0d1-104">Step 1: Verify that SharePoint Designer 2013 is updated with [SharePoint Designer Service Pack 1](https://support.microsoft.com/help/2817441/description-of-microsoft-sharepoint-designer-2013-service-pack-1-sp1) and the [August 2, 2016 Update for SharePoint Designer 2013](https://support.microsoft.com/help/3114721/august-2-2016-update-for-sharepoint-designer-2013-kb3114721).</span></span>



<span data-ttu-id="cc0d1-105">Βήμα 2: Καταργήστε τα αρχεία της τοπικής μνήμης προσωρινής αποθήκευσης:</span><span class="sxs-lookup"><span data-stu-id="cc0d1-105">Step 2: Clear the local cache files:</span></span>

1. <span data-ttu-id="cc0d1-106">Κλείσιμο του SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-106">Close SharePoint Designer 2013.</span></span>

2. <span data-ttu-id="cc0d1-107">Στον τοπικό υπολογιστή, καταργήστε όλα τα αρχεία που βρέθηκαν σε κάθε έναν από τους παρακάτω φακέλους.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-107">On the local computer, remove all files found in each of the following folders.</span></span>

    - <span data-ttu-id="cc0d1-108">Extensions\Cache διακομιστής %APPDATA%\Microsoft\Web</span><span class="sxs-lookup"><span data-stu-id="cc0d1-108">%APPDATA%\Microsoft\Web Server Extensions\Cache</span></span>
    - <span data-ttu-id="cc0d1-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span><span class="sxs-lookup"><span data-stu-id="cc0d1-109">%APPDATA%\Microsoft\SharePoint Designer\ProxyAssemblyCache</span></span>
    - <span data-ttu-id="cc0d1-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span><span class="sxs-lookup"><span data-stu-id="cc0d1-110">%USERPROFILE%\AppData\Local\Microsoft\WebsiteCache</span></span>

3. <span data-ttu-id="cc0d1-111">Άνοιγμα του SharePoint Designer 2013 και εισαγάγετε το λογαριασμό ξανά, για να δείτε αν λειτουργεί.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-111">Open SharePoint Designer 2013 and enter the account again to see if it works.</span></span>

<span data-ttu-id="cc0d1-112">Βήμα 3: [Ενεργοποίηση σύγχρονη ελέγχου ταυτότητας για το Office 2013 σε συσκευές των Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="cc0d1-112">Step 3: [Enable Modern Authentication for Office 2013 on Windows Devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication?redirectSourcePath=/article/Enable-Modern-Authentication-for-Office-2013-on-Windows-devices-7dc1c01a-090f-4971-9677-f1b192d6c910&view=o365-worldwide).</span></span>

<span data-ttu-id="cc0d1-113">Βήμα 4: Οι διαχειριστές θα πρέπει να **Επιτρέψει προσαρμοσμένης δέσμης ενεργειών** με τις ρυθμίσεις του κέντρου διαχείρισης του SharePoint ώστε να επιτρέπεται η σύνδεση του SharePoint Designer.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-113">Step 4: Administrators will need to **Allow Custom Script** in the SharePoint Admin Center settings to allow the SharePoint Designer connection.</span></span> <span data-ttu-id="cc0d1-114">Ανατρέξτε στην ενότητα [επιτρέπεται ή να απαγορεύεται η προσαρμοσμένη δέσμη ενεργειών](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) για περισσότερες πληροφορίες.</span><span class="sxs-lookup"><span data-stu-id="cc0d1-114">See [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script) for more information.</span></span>


