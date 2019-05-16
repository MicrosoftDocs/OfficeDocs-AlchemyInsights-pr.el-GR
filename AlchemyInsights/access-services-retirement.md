---
title: Συνταξιοδότηση υπηρεσίες πρόσβασης
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 395dac6abf1562aa0da0b1d87eddd943affefc3f
ms.sourcegitcommit: b2c9202b94fa1ce73dbeb3e43b219ba07e46e7e3
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/14/2019
ms.locfileid: "33973920"
---
# <a name="access-services-retirement"></a><span data-ttu-id="309fa-102">Συνταξιοδότηση υπηρεσίες πρόσβασης</span><span class="sxs-lookup"><span data-stu-id="309fa-102">Access services retirement</span></span>

<span data-ttu-id="309fa-103">Αρχικά ανακοινώνεται στο MC97576, στο Μαρτίου 2017, και εξακολούθησε να επικοινωνούν μέσω στον τελευταίο χρόνο πρόσβαση σε υπηρεσίες είναι να αποσυρθεί από το Office 365.</span><span class="sxs-lookup"><span data-stu-id="309fa-103">As we originally announced in MC97576, in March 2017, and continued to communicate over the past year Access Services are being retired from Office 365.</span></span> <span data-ttu-id="309fa-104">Η επόμενη φάση αυτής της διαδικασίας θα είναι η κατάργηση των βάσεων δεδομένων της Access Web που χρησιμοποιούν λίστες του SharePoint τους υποκείμενη αποθήκευση δεδομένων.</span><span class="sxs-lookup"><span data-stu-id="309fa-104">The next phase in this process will be the removal of Access Web Databases that use SharePoint lists as their underlying data storage.</span></span>

## <a name="how-does-this-affect-me"></a><span data-ttu-id="309fa-105">Πώς επηρεάζει αυτό μου;</span><span class="sxs-lookup"><span data-stu-id="309fa-105">How does this affect me?</span></span>

<span data-ttu-id="309fa-106">Εκκίνηση του Ιουνίου 2019, θα σταματήσει η δημιουργία νέων βάσεων δεδομένων της Access στο SharePoint Online και τερματισμός της υπηρεσίας και τις υπόλοιπες εφαρμογές ως το 2020 Απριλίου.</span><span class="sxs-lookup"><span data-stu-id="309fa-106">Starting June 2019, we will stop creation of new Access databases in SharePoint Online and shut down the service and any remaining apps by April 2020.</span></span>

## <a name="what-do-i-need-to-do-to-prepare-for-this-change"></a><span data-ttu-id="309fa-107">Τι πρέπει να κάνετε για να προετοιμαστείτε για αυτήν την αλλαγή;</span><span class="sxs-lookup"><span data-stu-id="309fa-107">What do I need to do to prepare for this change?</span></span>

<span data-ttu-id="309fa-108">Σας προτείνουμε να δημιουργήσετε ένα σχέδιο μετάβασης για βάσεις δεδομένων web της Access της εταιρείας σας.</span><span class="sxs-lookup"><span data-stu-id="309fa-108">We encourage you to create a transition plan for your organization’s Access web databases.</span></span> <span data-ttu-id="309fa-109">"Διαχειριστές" να χρησιμοποιήσετε το [σαρωτή app πρόσβασης του SharePoint](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) για να αποκτήσετε έναν κατάλογο με τις εφαρμογές της Access που χρησιμοποιούν τις τοποθεσίες.</span><span class="sxs-lookup"><span data-stu-id="309fa-109">Admins can use the [SharePoint Access app scanner](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fgithub.com%2FSharePoint%2FPnP-Tools%2Ftree%2Fmaster%2FSolutions%2FSharePoint.AccessApp.Scanner&data=02%7C01%7Csalarson%40microsoft.com%7C0f8afc9cd02f45ac32d708d6d26c5b40%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636927760189423652&sdata=xH%2FPQdPyyGEUBiXfMwUAhBE4UmsuBa4JhFDZUbjUkZU%3D&reserved=0) to obtain an inventory of the Access apps that sites are using.</span></span> 

<span data-ttu-id="309fa-110">Υπάρχουν διάφοροι τρόποι για τη μετεγκατάσταση δεδομένων του Access web βάσεις δεδομένων:</span><span class="sxs-lookup"><span data-stu-id="309fa-110">There are several ways to migrate Access web databases data:</span></span>

- <span data-ttu-id="309fa-111">Εισαγωγή σε μια τοπική βάση δεδομένων της Access (. ACCDB) ή σε ένα αρχείο Excel.</span><span class="sxs-lookup"><span data-stu-id="309fa-111">Importing to a local Access database (.ACCDB) or to an Excel file.</span></span>
- <span data-ttu-id="309fa-112">Συνιστάται επίσης να Εξερεύνηση Microsoft PowerApps ως μια εναλλακτική πλατφόρμα για να δημιουργήσετε λύσεις χωρίς κώδικα επαγγελματικών για το web και φορητές συσκευές.</span><span class="sxs-lookup"><span data-stu-id="309fa-112">We also recommend exploring Microsoft PowerApps as an alternative platform to create no-code business solutions for web and mobile devices.</span></span>