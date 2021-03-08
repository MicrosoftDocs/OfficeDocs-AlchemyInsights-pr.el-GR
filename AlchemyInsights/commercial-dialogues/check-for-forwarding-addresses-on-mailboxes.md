---
title: Έλεγχος για προώθηση διευθύνσεων σε γραμματοκιβώτια
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482772"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="94154-102">Έλεγχος για προώθηση διευθύνσεων σε γραμματοκιβώτια</span><span class="sxs-lookup"><span data-stu-id="94154-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="94154-103">Μερικές φορές οι εισβολείς προωθεί τα μηνύματα ηλεκτρονικού ταχυδρομείου των χρηστών στον εαυτό τους, επομένως πρώτα θα ελέγξουμε για προώθηση διευθύνσεων και κανόνων στο γραμματοκιβώτιο.</span><span class="sxs-lookup"><span data-stu-id="94154-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="94154-104">Στη συνέχεια, θα ελέγξουμε τα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="94154-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="94154-105">Δείτε πώς μπορείτε να ελέγξετε για προώθηση διευθύνσεων:</span><span class="sxs-lookup"><span data-stu-id="94154-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="94154-106">Επιλέξτε χρήστες **που**  >  **είναι ενεργοί χρήστες.**</span><span class="sxs-lookup"><span data-stu-id="94154-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="94154-107">Επιλέξτε το χρήστη του οποίου ο λογαριασμός έχει παραβιαστεί.</span><span class="sxs-lookup"><span data-stu-id="94154-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="94154-108">Στο αναδυόμενο στοιχείο που εμφανίζεται, αναπτύξτε τις ρυθμίσεις **αλληλογραφίας και,** στη συνέχεια, κάντε κλικ στην επιλογή **"Επεξεργασία** **για προώθηση ηλεκτρονικού ταχυδρομείου".**</span><span class="sxs-lookup"><span data-stu-id="94154-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="94154-109">Καταργήστε τυχόν διευθύνσεις προώθησης που δεν αναγνωρίζετε.</span><span class="sxs-lookup"><span data-stu-id="94154-109">Remove any forwarding addresses you don't recognize.</span></span>