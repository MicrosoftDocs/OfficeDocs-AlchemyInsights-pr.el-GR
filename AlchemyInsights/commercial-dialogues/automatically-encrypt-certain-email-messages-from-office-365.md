---
title: Αυτόματη κρυπτογράφηση ορισμένων μηνυμάτων ηλεκτρονικού ταχυδρομείου από το Office 365
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000078"
- "7342"
ms.openlocfilehash: 5ddaaed361f6ec934cfffb00cc62a9df2d1a04e8
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746136"
---
# <a name="automatically-encrypt-certain-email-messages-from-office-365"></a><span data-ttu-id="5011a-102">Αυτόματη κρυπτογράφηση ορισμένων μηνυμάτων ηλεκτρονικού ταχυδρομείου από το Office 365</span><span class="sxs-lookup"><span data-stu-id="5011a-102">Automatically encrypt certain email messages from office 365</span></span>

1. <span data-ttu-id="5011a-103">Από το [κέντρο διαχείρισης του Exchange,](https://outlook.office365.com/ecp/)επιλέξτε **κανόνες ροής > αλληλογραφίας.**</span><span class="sxs-lookup"><span data-stu-id="5011a-103">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="5011a-104">Κάντε κλικ στο **εικονίδιο "Δημιουργία" (+)** και, στη συνέχεια, κάντε κλικ στην επιλογή "Εφαρμογή κρυπτογράφησης μηνυμάτων του **Office 365" και προστασία δικαιωμάτων σε μηνύματα.**</span><span class="sxs-lookup"><span data-stu-id="5011a-104">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="5011a-105">Στο **πεδίο "Όνομα",** πληκτρολογήστε ένα όνομα για τον κανόνα, όπως "Κρυπτογράφηση όλων των *μηνυμάτων".*</span><span class="sxs-lookup"><span data-stu-id="5011a-105">In **Name**, enter a name for the rule, such as *Encrypt all messages*.</span></span>
4. <span data-ttu-id="5011a-106">Στην **ενότητα "Εφαρμογή αυτού του κανόνα",** εάν , **επιλέξτε [Εφαρμογή σε όλα τα μηνύματα]**.</span><span class="sxs-lookup"><span data-stu-id="5011a-106">In **Apply this rule if**, choose **[Apply to all messages]**.</span></span> 
5. <span data-ttu-id="5011a-107">Δίπλα στο πεδίο **"Να γίνει το εξής",** κάντε κλικ **στην επιλογή "Επιλογή ενός".**</span><span class="sxs-lookup"><span data-stu-id="5011a-107">Next to the **Do the following** field, click **Select one**.</span></span> 
6. <span data-ttu-id="5011a-108">Στο αναπτυσσόμενο **μενού προτύπου RMS,** επιλέξτε "Κρυπτογράφηση" **και,** στη συνέχεια, κάντε κλικ στο **κουμπί OK.**</span><span class="sxs-lookup"><span data-stu-id="5011a-108">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="5011a-109">(Εάν δεν βλέπετε αυτή την επιλογή, αυτό σημαίνει ότι το σχέδιό σας δεν περιλαμβάνει αυτόματη κρυπτογράφηση.</span><span class="sxs-lookup"><span data-stu-id="5011a-109">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="5011a-110">Ωστόσο, μπορείτε να το προσθέσετε!)</span><span class="sxs-lookup"><span data-stu-id="5011a-110">But you can add it!)</span></span>
7. <span data-ttu-id="5011a-111">Επιλέξτε το **πλαίσιο ελέγχου "Έλεγχος αυτού του κανόνα με επίπεδο σοβαρότητας"** και, στη συνέχεια, επιλέξτε το επιθυμητό επίπεδο.</span><span class="sxs-lookup"><span data-stu-id="5011a-111">Check the **Audit this rule with severity level** check box, and then select the desired level.</span></span> <span data-ttu-id="5011a-112">Εάν η εταιρεία σας έχει συμβατικές υποχρεώσεις για την αποστολή κρυπτογραφημένων μηνυμάτων ηλεκτρονικού ταχυδρομείου, συνιστάται να ορίσετε το επίπεδο **σε "Υψηλή".**</span><span class="sxs-lookup"><span data-stu-id="5011a-112">If your company has contractual obligations to send all emails encrypted, I recommend setting the level to **High**.</span></span>
8. <span data-ttu-id="5011a-113">Στην **περιοχή "Επιλογή μοντέλου για αυτόν τον κανόνα", κάντε** κλικ στην επιλογή **"Επιβολή".**</span><span class="sxs-lookup"><span data-stu-id="5011a-113">Under **Choose a model for this rule**, click **Enforce**.</span></span> 
9. <span data-ttu-id="5011a-114">Επιλέξτε οποιαδήποτε προαιρετική επιλογή (από μια λίστα προαιρετικών επιλογών που μπορείτε να κάνετε σε αυτό το σημείο, πολλές από τις οποίες μπορεί να τίθενται με την προεπιλεγμένη ρύθμιση για απλότητα).</span><span class="sxs-lookup"><span data-stu-id="5011a-114">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="5011a-115">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="5011a-115">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="5011a-116">Μπορείτε πάντα να ξανάρθετε και να επεξεργαστείτε αυτόν τον κανόνα αργότερα.</span><span class="sxs-lookup"><span data-stu-id="5011a-116">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="5011a-117">Για περισσότερες πληροφορίες σχετικά με τη δημιουργία κανόνων κρυπτογράφησης, ανατρέξτε στο θέμα Ορισμός κανόνων ροής αλληλογραφίας για την κρυπτογράφηση μηνυμάτων [ηλεκτρονικού ταχυδρομείου στο Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="5011a-117">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span></span>

