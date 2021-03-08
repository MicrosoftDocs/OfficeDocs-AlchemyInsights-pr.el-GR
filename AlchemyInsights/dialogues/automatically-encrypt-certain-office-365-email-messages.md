---
title: Αυτόματη κρυπτογράφηση ορισμένων μηνυμάτων ηλεκτρονικού ταχυδρομείου του Office 365
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
ms.openlocfilehash: e4b2f4ffcacf03e145b4c6d5ff6e73a75cb7c184
ms.sourcegitcommit: c202c0df2d141e63f4f7eb13a56efbfc2f57348f
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/05/2021
ms.locfileid: "50524898"
---
# <a name="automatically-encrypt-certain-office-365-email-messages"></a><span data-ttu-id="68001-102">Αυτόματη κρυπτογράφηση ορισμένων μηνυμάτων ηλεκτρονικού ταχυδρομείου του Office 365</span><span class="sxs-lookup"><span data-stu-id="68001-102">Automatically encrypt certain Office 365 email messages</span></span>

<span data-ttu-id="68001-103">Μπορείτε να κρυπτογραφείτε αυτόματα τα μηνύματα που στέλνουν οι χρήστες σε συγκεκριμένα εξωτερικά άτομα ή εταιρείες.</span><span class="sxs-lookup"><span data-stu-id="68001-103">You can automatically encrypt messages that users send to certain external people or organizations.</span></span> <span data-ttu-id="68001-104">Για να το κάνετε αυτό, εκτελέστε τα ακόλουθα βήματα:</span><span class="sxs-lookup"><span data-stu-id="68001-104">To do this, perform the following steps:</span></span>

1. <span data-ttu-id="68001-105">Από το [κέντρο διαχείρισης του Exchange,](https://outlook.office365.com/ecp/)επιλέξτε **τους κανόνες ροής > αλληλογραφίας.**</span><span class="sxs-lookup"><span data-stu-id="68001-105">From the [Exchange admin center](https://outlook.office365.com/ecp/), choose **mail flow > rules**.</span></span> 
2. <span data-ttu-id="68001-106">Κάντε κλικ στο **εικονίδιο "Νέο" (+)** και, στη συνέχεια, κάντε κλικ στην επιλογή "Εφαρμογή κρυπτογράφησης μηνυμάτων και προστασίας δικαιωμάτων του **Office 365" σε μηνύματα.**</span><span class="sxs-lookup"><span data-stu-id="68001-106">Click the **New (+)** icon, and then click **Apply Office 365 Message Encryption and rights protection to messages**.</span></span>
3. <span data-ttu-id="68001-107">Στο **πεδίο "Όνομα",** πληκτρολογήστε ένα όνομα για τον κανόνα, όπως "Κρυπτογράφηση μηνυμάτων που αποστέλλονται *DrToniRamos@gmail.com"*.</span><span class="sxs-lookup"><span data-stu-id="68001-107">In **Name**, enter a name for the rule, such as *Encrypt messages sent to DrToniRamos@gmail.com*.</span></span>
4. <span data-ttu-id="68001-108">Στην **επιλογή "Εφαρμογή αυτού του κανόνα",** επιλέξτε **τον παραλήπτη > είναι αυτό το άτομο.**</span><span class="sxs-lookup"><span data-stu-id="68001-108">In **Apply this rule if**, choose **The recipient > is this person**.</span></span> 
5. <span data-ttu-id="68001-109">Στο παράθυρο **"Επιλογή μελών",** επιλέξτε το όνομα του ατόμου στο οποίο θέλετε να εφαρμοστεί ο κανόνας κρυπτογράφησης και, στη συνέχεια, κάντε κλικ στην επιλογή **"Προσθήκη".**</span><span class="sxs-lookup"><span data-stu-id="68001-109">In the **Select Members** window, select the name of the person you want the encryption rule to apply to, and then click **add**.</span></span> 
6. <span data-ttu-id="68001-110">Όταν τελειώσετε με την προσθήκη χρηστών, κάντε κλικ στο κουμπί **OK.**</span><span class="sxs-lookup"><span data-stu-id="68001-110">When you're done adding users, click **OK**.</span></span>
7. <span data-ttu-id="68001-111">Δίπλα στο πεδίο **"Κάντε το εξής",** κάντε κλικ **στην επιλογή "Επιλογή".**</span><span class="sxs-lookup"><span data-stu-id="68001-111">Next to the **Do the following** field, click **Select one**.</span></span> 
8. <span data-ttu-id="68001-112">Στο αναπτυσσόμενο μενού **προτύπου RMS,** επιλέξτε "Κρυπτογράφηση" **και,** στη συνέχεια, κάντε κλικ στο κουμπί **OK.**</span><span class="sxs-lookup"><span data-stu-id="68001-112">In the **RMS template** drop-down menu, select **Encrypt**, and then click **OK**.</span></span> <span data-ttu-id="68001-113">(Εάν δεν βλέπετε αυτή την επιλογή, αυτό σημαίνει ότι το σχέδιό σας δεν περιλαμβάνει αυτόματη κρυπτογράφηση.</span><span class="sxs-lookup"><span data-stu-id="68001-113">(If you don't see this option, it means your plan doesn't include automatic encryption.</span></span> <span data-ttu-id="68001-114">Ωστόσο, μπορείτε να το προσθέσετε!)</span><span class="sxs-lookup"><span data-stu-id="68001-114">But you can add it!)</span></span>
9. <span data-ttu-id="68001-115">Επιλέξτε οποιαδήποτε προαιρετική επιλογή (από μια λίστα προαιρετικών επιλογών που μπορείτε να κάνετε σε αυτό το σημείο, πολλές από τις οποίες μπορεί να τίθενται στην προεπιλεγμένη ρύθμιση για απλότητα).</span><span class="sxs-lookup"><span data-stu-id="68001-115">Choose any optional selection (from a list of optional selections that you can make at this point, many of which can be left with the default setting for simplicity).</span></span>
10. <span data-ttu-id="68001-116">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="68001-116">Click **Save**.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="68001-117">Μπορείτε πάντα να επιστρέψει και να επεξεργαστείτε αυτόν τον κανόνα αργότερα.</span><span class="sxs-lookup"><span data-stu-id="68001-117">You can always come back and edit this rule later.</span></span>

<span data-ttu-id="68001-118">Για περισσότερες πληροφορίες σχετικά με τη δημιουργία κανόνων για κρυπτογράφηση, ανατρέξτε στο θέμα "Ορισμός κανόνων ροής [αλληλογραφίας για την κρυπτογράφηση μηνυμάτων ηλεκτρονικού ταχυδρομείου στο Office 365".](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email)</span><span class="sxs-lookup"><span data-stu-id="68001-118">For more information about creating rules for encryption, see [Define mail flow rules to encrypt email messages in Office 365](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).</span></span>
