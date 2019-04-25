---
title: Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 45665f900014c52e6a920325b0a3b0f6f79fb72d
ms.sourcegitcommit: d1c1d5bcb52ba9083e8dd7603feb72436c5154c8
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31910599"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a><span data-ttu-id="8acc4-102">Επιδιορθώστε προβλήματα παράδοσης ηλεκτρονικού ταχυδρομείου για δημόσιους φακέλους με δυνατότητα αλληλογραφίας</span><span class="sxs-lookup"><span data-stu-id="8acc4-102">Fix email delivery issues to mail-enabled public folders</span></span>

<span data-ttu-id="8acc4-103">Εάν εξωτερικοί αποστολείς δεν είναι δυνατό να στείλετε μηνύματα στους δημόσιους φακέλους σας με δυνατότητα αλληλογραφίας και τους αποστολείς να εμφανιστεί το μήνυμα λάθους: **δεν ήταν δυνατή η εύρεση (550 5.4.1)**, επιβεβαιώστε τον τομέα ηλεκτρονικού ταχυδρομείου για τον δημόσιο φάκελο που έχει ρυθμιστεί ως μια εσωτερική αναμετάδοσης τομέα αντί για ένα επιτακτική τομέα:</span><span class="sxs-lookup"><span data-stu-id="8acc4-103">If external senders can't send messages to your mail-enabled public folders, and the senders receive the error: **couldn't be found (550 5.4.1)**, verify the email domain for the public folder is configured as an internal relay domain instead of an authoritative domain:</span></span>

1. <span data-ttu-id="8acc4-104">Ανοίξτε το [Κέντρο διαχείρισης Exchange (ΕΚΟ)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span><span class="sxs-lookup"><span data-stu-id="8acc4-104">Open the [Exchange admin center (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center).</span></span>

2. <span data-ttu-id="8acc4-105">Μεταβείτε στην **ροή αλληλογραφίας** \> **δεκτά τομέων**, επιλέξτε τον τομέα που έγινε αποδεκτή και, στη συνέχεια, κάντε κλικ στο κουμπί **Επεξεργασία**.</span><span class="sxs-lookup"><span data-stu-id="8acc4-105">Go to **Mail flow** \> **Accepted domains**, select the accepted domain, and then click **Edit**.</span></span>

3. <span data-ttu-id="8acc4-106">Στις ιδιότητες σελίδας που ανοίγει, εάν έχει οριστεί ο τύπος τομέα **Authoritative**, αλλάξτε την τιμή σε **εσωτερικό αναμετάδοσης** και, στη συνέχεια, κάντε κλικ στο κουμπί **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="8acc4-106">In the properties page that opens, if the domain type is set to **Authoritative**, change the value to **Internal relay** and then click **Save**.</span></span>

<span data-ttu-id="8acc4-107">Εάν εξωτερικοί αποστολείς, λαμβάνετε το σφάλμα που **δεν έχετε δικαίωμα (550 5.7.13)**, εκτελέστε την ακόλουθη εντολή στο [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) για να δείτε τα δικαιώματα για τους ανώνυμους χρήστες στο δημόσιο φάκελο:</span><span class="sxs-lookup"><span data-stu-id="8acc4-107">If external senders receive the error **you don't have permission (550 5.7.13)**, run the following command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell) to see the permissions for anonymous users in the public folder:</span></span>

<span data-ttu-id="8acc4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`Για παράδειγμα, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span><span class="sxs-lookup"><span data-stu-id="8acc4-108">`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous` For example, `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`.</span></span>

<span data-ttu-id="8acc4-109">Για να επιτρέπεται στους εξωτερικούς χρήστες να στείλετε μήνυμα ηλεκτρονικού ταχυδρομείου σε αυτόν τον δημόσιο φάκελο, προσθέστε την πρόσβαση CreateItems δεξιά ο ανώνυμος χρήστης.</span><span class="sxs-lookup"><span data-stu-id="8acc4-109">To allow external users to send email to this public folder, add the CreateItems access right to the user Anonymous.</span></span> <span data-ttu-id="8acc4-110">Για παράδειγμα, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span><span class="sxs-lookup"><span data-stu-id="8acc4-110">For example, `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`.</span></span>