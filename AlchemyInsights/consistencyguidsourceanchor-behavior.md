---
title: ConsistencyGuid / sourceAnchor συμπεριφορά
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659591"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="7844e-102">ConsistencyGuid / sourceAnchor συμπεριφορά</span><span class="sxs-lookup"><span data-stu-id="7844e-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="7844e-p101">Σύνδεση AD Azure (έκδοση 1.1.524.0 και μετά) τώρα διευκολύνει τη χρήση msDS-ConsistencyGuid ως χαρακτηριστικό sourceAnchor. Όταν χρησιμοποιείτε αυτήν τη δυνατότητα, σύνδεση AD Azure ρυθμίζει αυτόματα τις παραμέτρους των κανόνων συγχρονισμού για να:</span><span class="sxs-lookup"><span data-stu-id="7844e-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="7844e-p102">Χρησιμοποιήστε msDS-ConsistencyGuid με το χαρακτηριστικό sourceAnchor για αντικείμενα χρήστη. ObjectGUID χρησιμοποιείται για άλλους τύπους αντικειμένου.</span><span class="sxs-lookup"><span data-stu-id="7844e-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="7844e-p103">Για οποιαδήποτε λόγω εσωτερικής εγκατάστασης χρήστη AD αντικείμενο του οποίου το χαρακτηριστικό msDS-ConsistencyGuid δεν είναι συμπληρωμένη, Azure AD σύνδεση εγγράφει την τιμή objectGUID πίσω στο χαρακτηριστικό msDS-ConsistencyGuid εσωτερικής εγκατάστασης υπηρεσίας καταλόγου Active Directory. Αφού συμπληρωθεί το χαρακτηριστικό msDS-ConsistencyGuid, σύνδεση AD Azure εξάγει, στη συνέχεια, το αντικείμενο Azure AD.</span><span class="sxs-lookup"><span data-stu-id="7844e-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="7844e-p104">**Σημείωση:** Μία φορά μια ενδοεταιρική αντικείμενο AD εισάγεται στη σύνδεση AD Azure (δηλαδή, εισάγονται στο χώρο της σύνδεσης AD και πρόβλεψη σε το Metaverse), δεν μπορείτε να αλλάξετε την τιμή της sourceAnchor πλέον. Για να καθορίσετε την τιμή sourceAnchor για μια λόγω εσωτερικής εγκατάστασης AD αντικειμένων, να ρυθμίσετε τις παραμέτρους του χαρακτηριστικού msDS-ConsistencyGuid, πριν από την εισαγωγή σε σύνδεση AD Azure.</span><span class="sxs-lookup"><span data-stu-id="7844e-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="7844e-111">Για περισσότερες πληροφορίες σχετικά με SourceAnchor και ConsistencyGuid, ανατρέξτε στα παρακάτω: [σύνδεση AD Azure: Σχεδίαση έννοιες](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="7844e-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  
