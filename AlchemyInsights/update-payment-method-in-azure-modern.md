---
title: Ενημέρωση λεπτομερειών πληρωμής στο Azure (μοντέρνο)
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 82c0a06e-86b0-4e8c-8644-59cbc02e7645
ms.custom:
- "9003546"
- "6857"
ms.openlocfilehash: bb032f772077318e54ac4fde42a72f432703d828
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807506"
---
# <a name="update-payment-details-in-azure"></a><span data-ttu-id="72fe4-102">Ενημέρωση λεπτομερειών πληρωμής στο Azure</span><span class="sxs-lookup"><span data-stu-id="72fe4-102">Update payment details in Azure</span></span>

<span data-ttu-id="72fe4-103">Εάν η πιστωτική κάρτα ανανεωθεί και ο αριθμός παραμείνει ο ίδιος, ενημερώστε τα υπάρχοντα στοιχεία της πιστωτικής κάρτας, όπως η ημερομηνία λήξης.</span><span class="sxs-lookup"><span data-stu-id="72fe4-103">If your credit card gets renewed and the number stays the same, update the existing credit card details like the expiration date.</span></span> <span data-ttu-id="72fe4-104">Εάν ο αριθμός της πιστωτικής σας κάρτας αλλάξει, επειδή η κάρτα έχει χαθεί, κλαπεί ή λήξει, ακολουθήστε τα βήματα στην ενότητα [Προσθήκη πιστωτικής κάρτας ως μεθόδου πληρωμής](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) .</span><span class="sxs-lookup"><span data-stu-id="72fe4-104">If your credit card number changes because the card is lost, stolen, or expired, follow the steps in the [Add a credit card as a payment method](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#addcard) section.</span></span> <span data-ttu-id="72fe4-105">Δεν χρειάζεται να ενημερώσετε το κωδικού CVV.</span><span class="sxs-lookup"><span data-stu-id="72fe4-105">You don't need to update the CVV.</span></span>

<span data-ttu-id="72fe4-106">Οι μέθοδοι πληρωμής σας σχετίζονται με τα [προφίλ χρέωσης](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span><span class="sxs-lookup"><span data-stu-id="72fe4-106">Your Payment methods are associated with [billing profiles](https://docs.microsoft.com/azure/billing/billing-how-to-change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support#change-payment-method-for-a-billing-profile).</span></span> <span data-ttu-id="72fe4-107">Μόνο ο χρήστης που υπέγραψε για το Azure και δημιούργησε τον λογαριασμό χρέωσης μπορεί να ενημερώσει τον τρόπο πληρωμής.</span><span class="sxs-lookup"><span data-stu-id="72fe4-107">Only the user who signed up for Azure and created the billing account can update the payment method.</span></span> <span data-ttu-id="72fe4-108">Ακολουθήστε τα παρακάτω βήματα για να ενημερώσετε τον τρόπο πληρωμής.</span><span class="sxs-lookup"><span data-stu-id="72fe4-108">Follow these steps to update the payment method.</span></span>

1. <span data-ttu-id="72fe4-109">Πραγματοποιήστε είσοδο στην [πύλη Azure](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="72fe4-109">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>

2. <span data-ttu-id="72fe4-110">Αναζητήστε τη **Διαχείριση κόστους + χρέωση** .</span><span class="sxs-lookup"><span data-stu-id="72fe4-110">Search on **Cost Management + Billing** .</span></span>

3. <span data-ttu-id="72fe4-111">Στο μενού στα αριστερά, επιλέξτε **προφίλ χρέωσης** .</span><span class="sxs-lookup"><span data-stu-id="72fe4-111">In the menu on the left, select **Billing profiles** .</span></span>

4. <span data-ttu-id="72fe4-112">Επιλέξτε ένα προφίλ χρέωσης.</span><span class="sxs-lookup"><span data-stu-id="72fe4-112">Select a billing profile.</span></span>

5. <span data-ttu-id="72fe4-113">Στο μενού στα αριστερά, επιλέξτε **μέθοδοι πληρωμής** .</span><span class="sxs-lookup"><span data-stu-id="72fe4-113">In the menu on the left, select **Payment methods** .</span></span>

6. <span data-ttu-id="72fe4-114">Στην ενότητα οι **πιστωτικές κάρτες σας** , εντοπίστε την πιστωτική κάρτα που θέλετε να επεξεργαστείτε.</span><span class="sxs-lookup"><span data-stu-id="72fe4-114">In the **Your credit cards** section, find the credit card you want to edit.</span></span>
7. <span data-ttu-id="72fe4-115">Επιλέξτε την έλλειψη **(...)** στο άκρο της γραμμής.</span><span class="sxs-lookup"><span data-stu-id="72fe4-115">Select the ellipsis **(...)** at the end of the row.</span></span>

8. <span data-ttu-id="72fe4-116">Για να επεξεργαστείτε τα στοιχεία της πιστωτικής σας κάρτας, επιλέξτε  **Επεξεργασία**  από το μενού περιβάλλοντος.</span><span class="sxs-lookup"><span data-stu-id="72fe4-116">To edit your credit card details, select  **Edit**  from the context menu.</span></span>
