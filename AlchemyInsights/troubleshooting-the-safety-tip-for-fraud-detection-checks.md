---
title: Αντιμετώπιση προβλημάτων της συμβουλής ασφάλειας για την ανίχνευση της απάτης ελέγχει
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 96ebe3c5-66ea-4662-98b7-052c2181c2f3
ms.openlocfilehash: 06a0b5b8d29052e6033de5938b8ea67ceabc9848
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29658115"
---
# <a name="troubleshooting-the-safety-tip-for-fraud-detection-checks"></a><span data-ttu-id="de443-102">Αντιμετώπιση προβλημάτων της συμβουλής ασφάλειας για την ανίχνευση της απάτης ελέγχει</span><span class="sxs-lookup"><span data-stu-id="de443-102">Troubleshooting the safety tip for fraud detection checks</span></span>



<span data-ttu-id="de443-p101">Εάν είστε γρήγορα μια συμβουλή ασφαλείας που αναφέρει ότι "ο αποστολέας απέτυχε μας έλεγχοι εντοπισμού της απάτης και ενδέχεται να μην είναι που να εμφανίζονται ως" και, στη συνέχεια, ο αποστολέας δεν μπόρεσε να περάσει έλεγχο ταυτότητας DKIM ή SPF. Είναι η καλύτερη μέθοδος για να επιλύσετε αυτό το θέμα για τον αποστολέα για να εξουσιοδοτήσετε τους. Εάν ο αποστολέας στέλνει για λογαριασμό σας, θα πρέπει να επιτρέπουν τους, προσθέτοντας τη διεύθυνση IP του αποστολέα για την καρτέλα σας SPF.</span><span class="sxs-lookup"><span data-stu-id="de443-p101">If you are getting a safety tip that says "The sender failed our fraud detection checks and may not be who they appear to be", then the sender failed to pass either DKIM or SPF authentication checks. The best method to resolve this is for the sender to authorize themselves. If the sender is sending on your behalf, you need to authorize them by adding the sender's IP address to your SPF record.</span></span>
  
<span data-ttu-id="de443-106">Για περισσότερες πληροφορίες, ανατρέξτε στο θέμα [Αντιμετώπιση προβλημάτων της συμβουλής κόκκινο ασφάλειας (ύποπτες) για την ανίχνευση της απάτης ελέγχει](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) .</span><span class="sxs-lookup"><span data-stu-id="de443-106">See [Troubleshooting the red (suspicious) safety tip for fraud detection checks](https://blogs.msdn.microsoft.com/tzink/2016/11/02/troubleshooting-the-red-suspicious-safety-tip-for-fraud-detection-checks/) for more info.</span></span> 
  
<span data-ttu-id="de443-107">Ακολουθούν ορισμένες άλλες συνδέσεις που μπορούν να σας βοηθήσουν:</span><span class="sxs-lookup"><span data-stu-id="de443-107">Here are some other links that can help:</span></span>
  
- [<span data-ttu-id="de443-108">Πώς το Office 365 χρησιμοποιεί αποστολέας πλαίσιο πολιτικής (SPF) για να αποτρέψετε την πλαστογράφηση</span><span class="sxs-lookup"><span data-stu-id="de443-108">How Office 365 uses sender policy framework (SPF) to prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/how-office-365-uses-spf-to-prevent-spoofing)
    
- [<span data-ttu-id="de443-109">Ορίσετε SPF στο Office 365, για να αποτραπεί η πλαστογράφηση</span><span class="sxs-lookup"><span data-stu-id="de443-109">Set up SPF in Office 365 to help prevent spoofing</span></span>](https://docs.microsoft.com/office365/SecurityCompliance/set-up-spf-in-office-365-to-help-prevent-spoofing)
    
