---
title: Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 3e88e0f3-c86d-4ab8-b076-59d0552318f9
ms.openlocfilehash: c16b7ac7d79794307fa33ed1039305ed5b842cf6
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/24/2019
ms.locfileid: "29471357"
---
# <a name="questions-about-how-to-use-the-office-deployment-tool-odt"></a><span data-ttu-id="cd30c-102">Ερωτήσεις σχετικά με τον τρόπο χρήσης του Office ανάπτυξης Tool (ODT)</span><span class="sxs-lookup"><span data-stu-id="cd30c-102">Questions about how to use the Office Deployment Tool (ODT)</span></span>

<span data-ttu-id="cd30c-103">Κάντε λήψη του εργαλείου ανάπτυξης του Office από το [Κέντρο λήψης της Microsoft](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span><span class="sxs-lookup"><span data-stu-id="cd30c-103">Download the Office Deployment Tool from the [Microsoft Download Center](http://go.microsoft.com/fwlink/p/?LinkID=626065).</span></span>
  
<span data-ttu-id="cd30c-104">Μετά τη λήψη του αρχείου, εκτελέστε το αυτοαποσυμπιεζόμενο εκτελέσιμο αρχείο, που περιέχει το Office εργαλείο ανάπτυξης εκτελέσιμο (setup.exe) και ένα αρχείο ρύθμισης παραμέτρων δείγματος (configuration.xml).</span><span class="sxs-lookup"><span data-stu-id="cd30c-104">After downloading the file, run the self-extracting executable file, which contains the Office Deployment Tool executable (setup.exe) and a sample configuration file (configuration.xml).</span></span>
  
 <span data-ttu-id="cd30c-105">**Για να αποκλείσετε ή να καταργήσετε τα προϊόντα του Office 365 ProPlus από υπολογιστές-πελάτες:**</span><span class="sxs-lookup"><span data-stu-id="cd30c-105">**To exclude or remove Office 365 ProPlus products from client computers:**</span></span>
  
<span data-ttu-id="cd30c-p101">Κατά την εγκατάσταση του Office 365 ProPlus, μπορείτε να εξαιρέσετε συγκεκριμένα προϊόντα. Για να γίνει αυτό, ακολουθήστε τα βήματα για την εγκατάσταση του Office με το ODT, αλλά περιλαμβάνει το στοιχείο ExcludeApp στο αρχείο ρύθμισης παραμέτρων. Για παράδειγμα, αυτό το αρχείο παραμέτρων εγκαθιστά όλα τα προϊόντα του Office 365 ProPlus εκτός από το Publisher:</span><span class="sxs-lookup"><span data-stu-id="cd30c-p101">When installing Office 365 ProPlus, you can exclude specific products. To do so, follow the steps for installing Office with the ODT, but include the ExcludeApp element in your configuration file. For example, this configuration file installs all the Office 365 ProPlus products except Publisher:</span></span>
  
```
<Add SourcePath="\\Server\share" Version="15.1.2.3" OfficeClientEdition="32">
    <Product ID="O365ProPlusRetail" >
      <Language ID="en-us" />
      <ExcludeApp ID="Publisher" />
    </Product>
</Add>
```

[<span data-ttu-id="cd30c-109">Επισκόπηση του εργαλείου ανάπτυξης του Office</span><span class="sxs-lookup"><span data-stu-id="cd30c-109">Overview of the Office Deployment Tool</span></span>](https://docs.microsoft.com/deployoffice/overview-of-the-office-2016-deployment-tool)
  
