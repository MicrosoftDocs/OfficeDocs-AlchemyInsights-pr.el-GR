---
title: Χρήση πολιτικών και σχέσεων οργανισμού του PowerShell για κοινή χρήση
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3800014"
- "898"
ms.openlocfilehash: 717cdd6827e243ac6bf375209a911937c97088d2
ms.sourcegitcommit: 722e9a0ed058cb1eab2dd053be2418b60f7d4aac
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44862086"
---
# <a name="use-powershell-for-sharing-policies-and-organization-relationships"></a><span data-ttu-id="b28a6-102">Χρήση πολιτικών και σχέσεων οργανισμού του PowerShell για κοινή χρήση</span><span class="sxs-lookup"><span data-stu-id="b28a6-102">Use PowerShell for Sharing policies and Organization relationships</span></span>


<span data-ttu-id="b28a6-103">Για σχέσεις οργανισμού, ανατρέξτε στις λεπτομερείς πληροφορίες σύνταξης και παραμέτρων για : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship) ΚΑΙ [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span><span class="sxs-lookup"><span data-stu-id="b28a6-103">For Organization relationships please review the detailed syntax and parameter information for : [Get-FederationInformation](https://docs.microsoft.com/powershell/module/exchange/get-federationinformation), [New-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/new-organizationrelationship), [Set-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/set-organizationrelationship)  AND  [Remove-OrganizationRelationship](https://docs.microsoft.com/powershell/module/exchange/remove-organizationrelationship).</span></span>

<span data-ttu-id="b28a6-104">Για να δημιουργήσετε πολιτική κοινής χρήσης, χρησιμοποιήστε [την Πολιτική νέας κατανομής](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b28a6-104">To create sharing policy use [New-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/new-sharingpolicy).</span></span> <span data-ttu-id="b28a6-105">Για να [εφαρμόσετε μια πολιτική κοινής χρήσης σε ένα γραμματοκιβώτιο ή χρήστη,](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes) πρέπει να χρησιμοποιήσετε ένα συνδυασμό [set-mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) και [get-mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) με τη νέα πολιτική.</span><span class="sxs-lookup"><span data-stu-id="b28a6-105">To  [apply a sharing policy to a mailbox or user](https://docs.microsoft.com/exchange/sharing/sharing-policies/apply-a-sharing-policy%23use-exchange-online-powershell-to-apply-a-sharing-policy-to-one-or-more-mailboxes)  you need to use a combination of  [Set-Mailbox](https://docs.microsoft.com/powershell/module/exchange/set-mailbox) and [Get-Mailbox](https://docs.microsoft.com/powershell/module/exchange/get-mailbox) with the newly created policy.</span></span> <span data-ttu-id="b28a6-106">Για να [τροποποιήσετε, να απενεργοποιήσετε ή να καταργήσετε μια πολιτική κοινής χρήσης,](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy) πρέπει να χρησιμοποιήσετε την [Πολιτική κοινής χρήσης και](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) την πολιτική [κατάργησης κοινής χρήσης](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span><span class="sxs-lookup"><span data-stu-id="b28a6-106">To  [modify, disable or remove a sharing policy](https://docs.microsoft.com/exchange/sharing/sharing-policies/modify-a-sharing-policy)  you need to use  [Set-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/set-sharingpolicy) and [Remove-SharingPolicy](https://docs.microsoft.com/powershell/module/exchange/remove-sharingpolicy).</span></span>

<span data-ttu-id="b28a6-107">**Για την πλήρη κατανόηση αυτού του θέματος παρακαλούμε διαβάστε:**</span><span class="sxs-lookup"><span data-stu-id="b28a6-107">**For full understanding of this topic please read:**</span></span>

[<span data-ttu-id="b28a6-108">Κοινή χρήση στο Exchange Online</span><span class="sxs-lookup"><span data-stu-id="b28a6-108">Sharing in Exchange Online</span></span>](https://docs.microsoft.com/exchange/sharing/sharing)