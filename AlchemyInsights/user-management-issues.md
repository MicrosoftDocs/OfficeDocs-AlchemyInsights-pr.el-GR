---
title: Ζητήματα διαχείρισης χρηστών
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9209"
- "9005371"
ms.openlocfilehash: 4b61686381de0cafa38857ca7a96b3a81aa191ec
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036281"
---
# <a name="user-management-issues"></a><span data-ttu-id="57c2e-102">Ζητήματα διαχείρισης χρηστών</span><span class="sxs-lookup"><span data-stu-id="57c2e-102">User management issues</span></span>

<span data-ttu-id="57c2e-103">**Τι συμβαίνει με τους τρέχοντες χρήστες που έχουν εκχωρηθεί στην εφαρμογή εάν απενεργοποιήσω την ιδιότητα "Απαιτείται ανάθεση χρήστη" (ορίστε αυτή την ιδιότητα σε "Όχι";**</span><span class="sxs-lookup"><span data-stu-id="57c2e-103">**What happens to current assigned users to the application if I disable the property ‘User assignment required’ (set this property to No)?**</span></span>

<span data-ttu-id="57c2e-104">Η απενεργοποίηση της **απαιτούμενης ανάθεσης εργασίας** χρήστη ΔΕΝ επηρεάζει τους χρήστες που έχουν αντιστοιχιστεί τη συγκεκριμένη στιγμή.</span><span class="sxs-lookup"><span data-stu-id="57c2e-104">Disabling **User assignment required** does NOT affect the currently assigned users.</span></span> <span data-ttu-id="57c2e-105">Η απενεργοποίηση αυτής της ιδιότητας θα επιτρέψει μόνο σε όλους τους χρήστες να αποκτήσουν πρόσβαση στην εφαρμογή.</span><span class="sxs-lookup"><span data-stu-id="57c2e-105">Disabling this property will only allow all users to access the application.</span></span> <span data-ttu-id="57c2e-106">Όλοι οι χρήστες που παρατίθενται και οι χρήστες που έχουν αντιστοιχιστεί σε ομάδες στην εφαρμογή θα εξακολουθούν να είναι έγκυροι.</span><span class="sxs-lookup"><span data-stu-id="57c2e-106">All the listed users and those users assigned to groups in the application will still be valid.</span></span>

- <span data-ttu-id="57c2e-107">Για να περιορίσετε την εφαρμογή σας σε συγκεκριμένο σύνολο χρηστών, ανατρέξτε στο θέμα - Περιορισμός εφαρμογής Azure AD σε ένα σύνολο χρηστών [- Πλατφόρμα ταυτότητας της Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span><span class="sxs-lookup"><span data-stu-id="57c2e-107">To restrict your app to specific set of users, see - [Restrict Azure AD app to a set of users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-restrict-your-app-to-a-set-of-users#:~:text=Select%20the%20application%20you%20want%2cand%20set%20it%20to%20Yes.).</span></span>
- <span data-ttu-id="57c2e-108">Για να εκχωρήσετε χρήστες και ομάδες, σε εταιρικές εφαρμογές στο Azure Active Directory (Azure AD), είτε μέσα από την πύλη Azure είτε χρησιμοποιώντας το PowerShell, ανατρέξτε στο θέμα Διαχείριση ανάθεσης χρηστών για μια εφαρμογή [στο Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal)</span><span class="sxs-lookup"><span data-stu-id="57c2e-108">To assign users and groups, to enterprise applications in Azure Active Directory (Azure AD), either from within the Azure portal or by using PowerShell, see [Manage user assignment for an app in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/assign-user-or-group-access-portal).</span></span>
- <span data-ttu-id="57c2e-109">Για να αναθέσετε δικαιώματα δημιουργίας και διαχείρισης εφαρμογών, ανατρέξτε στο θέμα Δικαιώματα διαχειριστή εφαρμογών [πληρεξουσίου - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span><span class="sxs-lookup"><span data-stu-id="57c2e-109">To delegate Application creation and management permissions, see [Delegate application management administrator permissions - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/roles/delegate-app-roles).</span></span>
- <span data-ttu-id="57c2e-110">**Απόκρυψη συγκεκριμένων εταιρικών εφαρμογών από χρήστες** - Ακολουθήστε τα παρακάτω βήματα για να αποκρύψετε όλες τις εφαρμογές του Microsoft 365 από τον **πίνακα MyApps.**</span><span class="sxs-lookup"><span data-stu-id="57c2e-110">**Hide specific enterprise apps from users** - Use the following steps to hide all Microsoft 365 apps from the **MyApps** panel.</span></span> <span data-ttu-id="57c2e-111">Οι εφαρμογές θα εξακολουθούν να είναι ορατές στην πύλη του Office 365.</span><span class="sxs-lookup"><span data-stu-id="57c2e-111">The apps will still be visible in the Office 365 portal.</span></span>

 1. <span data-ttu-id="57c2e-112">Πραγματοποιήστε είσοδο στην πύλη Azure ως καθολικός διαχειριστής για τον κατάλογο.</span><span class="sxs-lookup"><span data-stu-id="57c2e-112">Sign-in to the Azure portal as a global administrator for your directory.</span></span> 
 2. <span data-ttu-id="57c2e-113">Επιλέξτε **Azure Active Directory.**</span><span class="sxs-lookup"><span data-stu-id="57c2e-113">Select **Azure Active Directory**.</span></span> 
 3. <span data-ttu-id="57c2e-114">Επιλέξτε **"Χρήστες".**</span><span class="sxs-lookup"><span data-stu-id="57c2e-114">Select **Users**.</span></span> 
 4. <span data-ttu-id="57c2e-115">Επιλέξτε **"Ρυθμίσεις χρήστη".**</span><span class="sxs-lookup"><span data-stu-id="57c2e-115">Select **User settings**.</span></span> 
 5. <span data-ttu-id="57c2e-116">Στην περιοχή **"Εταιρικές εφαρμογές",** κάντε **κλικ στην επιλογή "Διαχείριση του πώς οι τελικοί χρήστες εκκινούν και προβάλλουν τις εφαρμογές τους".**</span><span class="sxs-lookup"><span data-stu-id="57c2e-116">Under **Enterprise applications**, click **Manage how end users launch and view their applications**.</span></span> 
 6. <span data-ttu-id="57c2e-117">Για **τους χρήστες μπορούν να δουν μόνο τις εφαρμογές του Office 365 στην πύλη του Office 365, κάντε κλικ** στο κουμπί **"Ναι".**</span><span class="sxs-lookup"><span data-stu-id="57c2e-117">For **Users can only see Office 365 apps in the Office 365 portal**, click **Yes**.</span></span> 
 7. <span data-ttu-id="57c2e-118">Επιλέξτε **Αποθήκευση**.</span><span class="sxs-lookup"><span data-stu-id="57c2e-118">Click **Save**.</span></span> 
 8. <span data-ttu-id="57c2e-119">Για περισσότερες λεπτομέρειες, [ανατρέξτε στο θέμα Απόκρυψη εταιρικής εφαρμογής από την εμπειρία χρήστη στο Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span><span class="sxs-lookup"><span data-stu-id="57c2e-119">For more details, see [Hide an Enterprise application from user's experience in Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/hide-application-from-user-portal#:~:text=%20Hide%20an%20application%20from%20the%20end%20user,6%20Click%20Properties.%207%20Click%20Save.%20See%20More.)</span></span>

- <span data-ttu-id="57c2e-120">Εάν προσφέρετε μια εφαρμογή Λογισμικού ως υπηρεσία (SaaS) σε πολλούς οργανισμούς, μπορείτε να ρυθμίσετε τις παραμέτρους της εφαρμογής σας ώστε να αποδέχεται τις είσοδοι από οποιονδήποτε μισθωτή azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="57c2e-120">If you offer a Software as a Service (SaaS) app to many organizations, you can configure your app to accept sign-ins from any Azure Active Directory (Azure AD) tenant.</span></span> <span data-ttu-id="57c2e-121">Αυτή η ρύθμιση παραμέτρων ονομάζεται "δημιουργία πολλών μισθωτών της εφαρμογής σας".</span><span class="sxs-lookup"><span data-stu-id="57c2e-121">This configuration is called "making your application multi-tenant".</span></span> <span data-ttu-id="57c2e-122">Οι χρήστες σε οποιονδήποτε μισθωτή του Azure AD θα μπορούν να πραγματοποιήσουν είσοδο στην εφαρμογή σας αφού συναινέσει στη χρήση του λογαριασμού τους με την εφαρμογή σας.</span><span class="sxs-lookup"><span data-stu-id="57c2e-122">Users in any Azure AD tenant will be able to sign-in to your app after consenting to use their account with your app.</span></span> <span data-ttu-id="57c2e-123">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα Δημιουργία εφαρμογών που θα πραγματοποιήσουν είσοδο σε χρήστες [του Azure AD - Πλατφόρμα ταυτότητας της Microsoft | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span><span class="sxs-lookup"><span data-stu-id="57c2e-123">For more information, see [Build apps that sign in Azure AD users - Microsoft identity platform | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant).</span></span>

- <span data-ttu-id="57c2e-124">**Πώς μπορεί ένας τελικός χρήστης να αποκτήσει πρόσβαση στην εφαρμογή μετά την εκχωρήσεή του στην εφαρμογή;**</span><span class="sxs-lookup"><span data-stu-id="57c2e-124">**How can an end user access the application once he/she is assigned to the application?**</span></span>

<span data-ttu-id="57c2e-125">Κάθε εφαρμογή στο Enterprise Application Blade διαθέτει μια σύνδεση για πρόσβαση στους τελικούς χρήστες.</span><span class="sxs-lookup"><span data-stu-id="57c2e-125">Each app in Enterprise application blade has a link for end users to access.</span></span> <span data-ttu-id="57c2e-126">Οι χρήστες μπορούν επίσης να αποκτήσουν πρόσβαση στην **εφαρμογή μέσω της πύλης Myapps** με εύκολο τρόπο.</span><span class="sxs-lookup"><span data-stu-id="57c2e-126">Users can also access the app through **Myapps** portal in an easy way.</span></span>

- <span data-ttu-id="57c2e-127">**Θέλετε να μάθετε ποιες εφαρμογές και τον τύπο εφαρμογών χρησιμοποιούνται από τους χρήστες;**</span><span class="sxs-lookup"><span data-stu-id="57c2e-127">**Want to know which applications and type of applications are being used by users?**</span></span>

<span data-ttu-id="57c2e-128">Μπορείτε να κάνετε λήψη αναφορών σύνδεσης για τις τελευταίες 30 ημέρες **από portal.azure.com > Azure Active directory> signins> να κάνετε λήψη αναφορών.**</span><span class="sxs-lookup"><span data-stu-id="57c2e-128">You can download sign-in reports for the last 30 days from **portal.azure.com > Azure Active directory> Signins> download reports**.</span></span>

- <span data-ttu-id="57c2e-129">Μάθετε πώς μπορείτε να [εκχωρήσετε σε ένα μισθωτή ευρεία συγκατάθεση διαχειριστή σε μια εφαρμογή και να ρυθμίσετε](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) τον [τρόπο με τον οποίο οι τελικοί χρήστες συναινούν σε εφαρμογές.](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent)</span><span class="sxs-lookup"><span data-stu-id="57c2e-129">Learn how to [Grant tenant wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) and [Configure how end users consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent).</span></span>

- <span data-ttu-id="57c2e-130">Κατανοήστε [πώς λειτουργεί η συγκατάθεση](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) και [διαχειριστείτε τη συγκατάθεση για τις εφαρμογές.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests)</span><span class="sxs-lookup"><span data-stu-id="57c2e-130">Understand [how consent works](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) and [Manage consent to applications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests).</span></span>

