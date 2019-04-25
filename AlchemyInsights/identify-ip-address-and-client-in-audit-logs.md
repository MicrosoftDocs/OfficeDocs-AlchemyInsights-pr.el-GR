---
title: Προσδιορίστε τη διεύθυνση IP και υπολογιστή-πελάτη, αρχείων καταγραφής ελέγχου
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1367
ms.assetid: ''
ms.openlocfilehash: 7e30a638de5926aa11b8ae637613a48076d7bdc9
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909263"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="d59d4-102">Προσδιορίστε τη διεύθυνση IP και υπολογιστή-πελάτη, αρχείων καταγραφής ελέγχου</span><span class="sxs-lookup"><span data-stu-id="d59d4-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="d59d4-103">Η διεύθυνση IP που αντιστοιχεί σε μια δραστηριότητα από κάποιον χρήστη ή διαχειριστή εμφανίζεται στα αρχεία καταγραφής ελέγχου.</span><span class="sxs-lookup"><span data-stu-id="d59d4-103">The IP address that corresponds to an activity by a user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="d59d4-104">Καταγράφεται επίσης τις πληροφορίες προγράμματος-πελάτη.</span><span class="sxs-lookup"><span data-stu-id="d59d4-104">The client information is also logged.</span></span> <span data-ttu-id="d59d4-105">Ακολουθούν τα βήματα για τον προσδιορισμό των πληροφοριών αυτών</span><span class="sxs-lookup"><span data-stu-id="d59d4-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="d59d4-106">Συνδεθείτε με το [Κέντρο συμμόρφωσης του Office 365 ασφαλείας &](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d59d4-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d59d4-107">Κάντε κλικ στο κουμπί **Αναζήτηση και έρευνα** και επιλέξτε **Αναζήτηση αρχείου καταγραφής ελέγχου**.</span><span class="sxs-lookup"><span data-stu-id="d59d4-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

   <span data-ttu-id="d59d4-108">Εάν είστε ενδιαφέρονται για μια συγκεκριμένη δραστηριότητα, επιλέξτε το από τη λίστα " **δραστηριότητες** ".</span><span class="sxs-lookup"><span data-stu-id="d59d4-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="d59d4-109">Σε αντίθετη περίπτωση, θα επιστραφούν όλες οι δραστηριότητες για τον επιλεγμένο χρήστη (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="d59d4-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="d59d4-110">**Σημείωση**: ορισμένες δραστηριότητες ενδέχεται να μην είναι διαθέσιμη στο μενού " **δραστηριότητες** ". Ωστόσο, οι ελέγχου στοιχείων θα επιστραφεί εάν η **Εμφάνιση αποτελεσμάτων για όλες τις δραστηριότητες που** είναι επιλεγμένο (προεπιλεγμένη ρύθμιση).</span><span class="sxs-lookup"><span data-stu-id="d59d4-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="d59d4-111">Καθορίστε το όνομα χρήστη στο πεδίο " **χρήστες** ", επιλέξτε την περιοχή κατάλληλη ημερομηνία για τη δραστηριότητα και, στη συνέχεια, κάντε κλικ στο κουμπί **Αναζήτηση**.</span><span class="sxs-lookup"><span data-stu-id="d59d4-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="d59d4-112">Στα αποτελέσματα, μπορείτε να δείτε τη διεύθυνση IP για αυτήν τη δραστηριότητα στο παράθυρο αποτελεσμάτων.</span><span class="sxs-lookup"><span data-stu-id="d59d4-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="d59d4-113">Επιλέξτε την καρτέλα "Έλεγχος" για να δείτε λεπτομερείς πληροφορίες με την Ανάδυση **Λεπτομέρειες** (για παράδειγμα, πρόγραμμα-πελάτης, χρήστης που εκτέλεσε την ενέργεια, κ.λπ.).</span><span class="sxs-lookup"><span data-stu-id="d59d4-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="d59d4-114">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Εύρεση της διεύθυνσης IP του υπολογιστή που χρησιμοποιείται για πρόσβαση σε ένα λογαριασμό που έχει παραβιαστεί](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="d59d4-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>