---
title: Ημερήσια ηλεκτρονικού ταχυδρομείου έγινε υπέρβαση του ορίου. Αναστολή ροής εργασίας.
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: 802aba696da61be5f0a6c12072842cbc3cd96499
ms.sourcegitcommit: 407f6c1e82f1a0be5cf53301fbf03cd25dcbf0ee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 08/02/2019
ms.locfileid: "36059639"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a><span data-ttu-id="f2a9b-103">Υπέρβαση του ορίου ημερήσιων ηλεκτρονικού ταχυδρομείου.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-103">Daily email Limit Exceeded.</span></span> <span data-ttu-id="f2a9b-104">Αναστολή ροής εργασίας.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-104">Workflow is suspended.</span></span>

<span data-ttu-id="f2a9b-105">Αυτό το σφάλμα ενδέχεται να εμφανιστούν στα ακόλουθα σενάρια:</span><span class="sxs-lookup"><span data-stu-id="f2a9b-105">This error may be received in the following scenarios:</span></span>

- <span data-ttu-id="f2a9b-106">Μπορείτε να έχετε μια ροή εργασίας σε ηλεκτρονική SharePoint που χρησιμοποιεί το SharePoint 2010 ή τύπος πλατφόρμας ροής εργασίας του SharePoint 2013.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-106">You have a workflow in SharePoint Online that's using the SharePoint 2010 or SharePoint 2013 workflow platform type.</span></span>
- <span data-ttu-id="f2a9b-107">Η ροή εργασίας έχει ρυθμιστεί για να στείλετε ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερα από 200 χρήστες κάθε φορά, περισσότερες από 10.000 παραλήπτες ανά ημέρα είτε περισσότερα από 30 μηνύματα ανά λεπτό.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-107">The workflow is configured to send a custom email message to more than 200 users at a time, more than 10,000 recipients per day, or more than 30 messages per minute.</span></span>
- <span data-ttu-id="f2a9b-108">Κατά την εκτέλεση της ροής εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρήσετε την ακόλουθη συμπεριφορά:</span><span class="sxs-lookup"><span data-stu-id="f2a9b-108">When you run the workflow, the email message isn't sent, and you notice the following behavior:</span></span>
    - <span data-ttu-id="f2a9b-109">Χρήση του τύπου πλατφόρμα SharePoint 2013 μιας ροής εργασίας, μεταβείτε στη σελίδα " **Κατάσταση ροής εργασίας** ".</span><span class="sxs-lookup"><span data-stu-id="f2a9b-109">For a workflow using the SharePoint 2013 platform type, you browse to the **Workflow Status** page.</span></span> <span data-ttu-id="f2a9b-110">Στη σελίδα "Κατάσταση ροής εργασίας", η **Εσωτερική κατάσταση** έχει οριστεί σε **αποτελέσματα**και το παράθυρο πληροφοριών εμφανίζει **δεν είναι δυνατή η αποστολή σε παραλήπτη**.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-110">On the Workflow Status page, the **Internal Status** is set to **Started**, and the information balloon displays **Unable to send to a recipient**.</span></span>

<span data-ttu-id="f2a9b-111">Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τις παραμέτρους ροής εργασίας για να στείλετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβαίνουν το [Exchange Online όρια του αποστολέα](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span><span class="sxs-lookup"><span data-stu-id="f2a9b-111">To work around this issue, configure your workflow to send email messages without exceeding the [Exchange Online sender limits](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits).</span></span> <span data-ttu-id="f2a9b-112">Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλετε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα Office 365, μια ομάδα διανομής ή ομάδα ασφαλείας αλληλογραφίας ενεργοποιημένη ή στείλτε το μήνυμα σε λιγότερα από 200 παραλήπτες ταυτόχρονα.</span><span class="sxs-lookup"><span data-stu-id="f2a9b-112">For example, use a pause in the workflow, send the email to an Office 365 group, a distribution group or mail enabled security group, or send the message to fewer than 200 recipients at a time.</span></span>


<span data-ttu-id="f2a9b-113">Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span><span class="sxs-lookup"><span data-stu-id="f2a9b-113">For more information, see the following [article](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).</span></span>

## <a name="related-topics"></a><span data-ttu-id="f2a9b-114">Σχετικά θέματα</span><span class="sxs-lookup"><span data-stu-id="f2a9b-114">Related topics</span></span>
- [<span data-ttu-id="f2a9b-115">Δημιουργία ροής</span><span class="sxs-lookup"><span data-stu-id="f2a9b-115">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="f2a9b-116">Του SharePoint και ροής</span><span class="sxs-lookup"><span data-stu-id="f2a9b-116">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 