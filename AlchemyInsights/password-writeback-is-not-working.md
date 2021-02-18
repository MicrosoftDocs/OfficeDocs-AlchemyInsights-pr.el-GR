---
title: Η Writeback κωδικού πρόσβασης δεν λειτουργεί
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 02/12/2021
ms.locfileid: "50243365"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="737bd-102">Η Writeback κωδικού πρόσβασης δεν λειτουργεί</span><span class="sxs-lookup"><span data-stu-id="737bd-102">Password Writeback is not working</span></span>

<span data-ttu-id="737bd-103">**Έχω προβλήματα με τη ρύθμιση των παραμέτρων της writeback κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="737bd-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="737bd-104">Η writeback κωδικού πρόσβασης είναι μια εξαιρετική δυνατότητα.</span><span class="sxs-lookup"><span data-stu-id="737bd-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="737bd-105">Βεβαιωθείτε ότι έχετε κατανοήσει τις απαιτήσεις άδειας χρήσης:</span><span class="sxs-lookup"><span data-stu-id="737bd-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="737bd-106">Πρέπει να έχετε εκχωρήσει τουλάχιστον μία άδεια χρήσης στον οργανισμό σας</span><span class="sxs-lookup"><span data-stu-id="737bd-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="737bd-107">**Χρήστες μόνο για cloud** - Οποιαδήποτε SKU επί πληρωμή για το Office 365 (O365) ή Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="737bd-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="737bd-108">**Χρήστες cloud ή/και** εσωτερικής εγκατάστασης - Azure AD Premium P1 ή P2, Φορητότητα για μεγάλες επιχειρήσεις + Ασφάλεια (EMS) ή Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="737bd-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="737bd-109">Για να μάθετε περισσότερα σχετικά με τις απαιτήσεις άδειας χρήσης, [ανατρέξτε στις απαιτήσεις παραχώρησης αδειών χρήσης για](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing) την επαναφορά κωδικού πρόσβασης από το χρήστη του Azure AD</span><span class="sxs-lookup"><span data-stu-id="737bd-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="737bd-110">Έχετε τουλάχιστον έναν λογαριασμό διαχειριστή και έναν δοκιμαστικό λογαριασμό χρήστη με μία από τις κατάλληλες άδειες χρήσης.</span><span class="sxs-lookup"><span data-stu-id="737bd-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="737bd-111">Πρέπει να συνδέσετε το Azure AD Connect στον πρωτεύοντα emulator ελεγκτή τομέα για να λειτουργήσει η επαναφορά του κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="737bd-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="737bd-112">Μπορείτε να ρυθμίσετε τις παραμέτρους του Azure AD Connect  ώστε να χρησιμοποιεί έναν πρωτεύοντα ελεγκτή τομέα κάνοντας δεξί κλικ στις ιδιότητες της σύνδεσης συγχρονισμού υπηρεσίας καταλόγου Active Directory και, στη συνέχεια, επιλέγοντας τις παραμέτρους **των διαμερισμάτων καταλόγου.**</span><span class="sxs-lookup"><span data-stu-id="737bd-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="737bd-113">Από εκεί, αναζητήστε την ενότητα **ρυθμίσεων σύνδεσης ελεγκτή τομέα και επιλέξτε** το πλαίσιο με τίτλο "Να **χρησιμοποιούνται μόνο οι προτιμώμενοι ελεγκτές τομέα".**</span><span class="sxs-lookup"><span data-stu-id="737bd-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="737bd-114">Εάν το προτιμώμενο DC δεν είναι ένας emulator PDC, το Azure AD Connect θα εξακολουθεί να έχει πρόσβαση στον PDC για την επαναφορά του κωδικού πρόσβασης.</span><span class="sxs-lookup"><span data-stu-id="737bd-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="737bd-115">Η επαναφορά κωδικού πρόσβασης έχει ρυθμιστεί και ενεργοποιηθεί στο μισθωτή σας.</span><span class="sxs-lookup"><span data-stu-id="737bd-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="737bd-116">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα ["Επιτρέψτε στους χρήστες να επαναφέρουν τους κωδικούς πρόσβασης του Azure AD"](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)που έχουν.</span><span class="sxs-lookup"><span data-stu-id="737bd-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="737bd-117">Βεβαιωθείτε ότι ο λογαριασμός διαχειριστή που χρησιμοποιείται για την ενεργοποίηση της δυνατότητας "Εγγραφή κωδικού πρόσβασης" είναι ένας λογαριασμός διαχειριστή cloud (δημιουργήθηκε στο Azure AD και όχι στο AD εσωτερικής εγκατάστασης)</span><span class="sxs-lookup"><span data-stu-id="737bd-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="737bd-118">Έχετε μια ανάπτυξη μεμονωμένου δάσους AD εσωτερικής εγκατάστασης που εκτελεί Windows Server 2008 R2, Windows Server 2012 ή Windows Server 2012 R2 με εγκατεστημένα τα πιο πρόσφατα service pack</span><span class="sxs-lookup"><span data-stu-id="737bd-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="737bd-119">Έχετε εγκαταστήσει το εργαλείο Azure AD Connect και έχετε προετοιμάσει το περιβάλλον AD για συγχρονισμό στο cloud.</span><span class="sxs-lookup"><span data-stu-id="737bd-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="737bd-120">Πριν από τη δοκιμή της writeback κωδικού πρόσβασης, βεβαιωθείτε ότι έχετε ολοκληρώσει πρώτα μια πλήρη εισαγωγή και πλήρη συγχρονισμό τόσο από το AD όσο και από το Azure AD στο Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="737bd-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="737bd-121">Για να μάθετε περισσότερα, δείτε πώς μπορείτε να κάνετε [πλήρη συγχρονισμό και πλήρη εισαγωγή στο Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="737bd-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="737bd-122">**Έχω πρόβλημα με τη συνδεσιμότητα με την επαναφορά κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="737bd-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="737bd-123">Λήψη και ενεργοποίηση της πιο πρόσφατης έκδοσης του [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="737bd-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="737bd-124">Ρύθμιση παραμέτρων τείχους προστασίας: Το εργαλείο Azure AD Connect (1.1.443 και άνω) θα χρειαστεί πρόσβαση **εξερχομένων HTTPS** σε:</span><span class="sxs-lookup"><span data-stu-id="737bd-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="737bd-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="737bd-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="737bd-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="737bd-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="737bd-127">Να επιτρέπεται η διατήρηση των αδρανών συνδέσεων για τουλάχιστον 2-3 λεπτά</span><span class="sxs-lookup"><span data-stu-id="737bd-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="737bd-128">**Εξακολουθώ να έχω προβλήματα με την επαναφορά του κωδικού πρόσβασης**</span><span class="sxs-lookup"><span data-stu-id="737bd-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="737bd-129">Εάν εξακολουθείτε να αντιμετωπίζετε δυσκολίες, δοκιμάστε να απενεργοποιήσετε και να ενεργοποιήσετε ξανά την υπηρεσία writeback κωδικού πρόσβασης στο εργαλείο Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="737bd-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="737bd-130">Για να μάθετε περισσότερα, δείτε πώς μπορείτε να [απενεργοποιήσετε και να ενεργοποιήσετε ξανά την writeback κωδικού πρόσβασης](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="737bd-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>