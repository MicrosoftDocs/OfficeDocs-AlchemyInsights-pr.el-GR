---
title: Σφάλμα του Teams 4c7
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3472"
- "9001211"
ms.openlocfilehash: 51f2aa936e803b63bcbdf73b89959cd3a1757751
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786669"
---
# <a name="4c7-error-in-microsoft-teams"></a><span data-ttu-id="cd4e7-102">Σφάλμα 4c7 στο Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="cd4e7-102">4c7 error in Microsoft Teams</span></span>

<span data-ttu-id="cd4e7-103">Αυτό το σφάλμα παρουσιάζεται επειδή το Microsoft Teams απαιτεί έλεγχο ταυτότητας forms.</span><span class="sxs-lookup"><span data-stu-id="cd4e7-103">This error occurs because Microsoft Teams requires Forms Authentication.</span></span> <span data-ttu-id="cd4e7-104">Όταν αναπτύσσετε τις υπηρεσίες Active Directory Federation Services (AD FS), ο έλεγχος ταυτότητας φορμών δεν ενεργοποιείται για το intranet από προεπιλογή.</span><span class="sxs-lookup"><span data-stu-id="cd4e7-104">When you deploy Active Directory Federation Services (AD FS), Forms Authentication is not enabled for the intranet by default.</span></span> <span data-ttu-id="cd4e7-105">Εάν αποτύχει ο ενσωματωμένος έλεγχος ταυτότητας των Windows, θα σας ζητηθεί να εισέλθετε χρησιμοποιώντας τον έλεγχο ταυτότητας φορμών.</span><span class="sxs-lookup"><span data-stu-id="cd4e7-105">If Windows Integrated Authentication fails, you are prompted to sign in by using Forms Authentication.</span></span>

<span data-ttu-id="cd4e7-106">Για να επιλύσετε αυτό το πρόβλημα, ενεργοποιήστε τον έλεγχο ταυτότητας φορμών χρησιμοποιώντας το συμπληρωματικό πρόγραμμα AD FS Microsoft Management Console (MMC) στον υπολογιστή που διαθέτει το τοπικό αντίγραφο της υπηρεσίας καταλόγου Active Directory.</span><span class="sxs-lookup"><span data-stu-id="cd4e7-106">To resolve this issue, enable Forms Authentication by using the AD FS Microsoft Management Console (MMC) snap-in on the computer that has the local copy of Active Directory.</span></span> <span data-ttu-id="cd4e7-107">Για να το κάνετε, ακολουθήστε αυτά τα βήματα:</span><span class="sxs-lookup"><span data-stu-id="cd4e7-107">To do this, follow these steps:</span></span> 

1. <span data-ttu-id="cd4e7-108">Στο παράθυρο περιήγησης, μεταβείτε στην επιλογή **"Πολιτικές ελέγχου ταυτότητας".**</span><span class="sxs-lookup"><span data-stu-id="cd4e7-108">In the navigation pane, browse to **Authentication Policies**.</span></span>
2. <span data-ttu-id="cd4e7-109">Στην **περιοχή "Ενέργειες"** στο παράθυρο λεπτομερειών, επιλέξτε "Επεξεργασία **καθολικού πρωτεύοντος ελέγχου ταυτότητας".**</span><span class="sxs-lookup"><span data-stu-id="cd4e7-109">Under **Actions** in the details pane, select **Edit Global Primary Authentication**.</span></span>
3. <span data-ttu-id="cd4e7-110">Στην καρτέλα **Intranet, επιλέξτε** "Έλεγχος **ταυτότητας φορμών".**</span><span class="sxs-lookup"><span data-stu-id="cd4e7-110">On the **Intranet** tab, select **Forms Authentication**.</span></span>
4. <span data-ttu-id="cd4e7-111">Επιλέξτε **OK** (ή **Εφαρμογή).**</span><span class="sxs-lookup"><span data-stu-id="cd4e7-111">Select **OK** (or **Apply**).</span></span>