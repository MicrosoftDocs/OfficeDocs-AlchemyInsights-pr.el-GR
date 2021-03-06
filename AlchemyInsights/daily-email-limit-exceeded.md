---
title: Υπέρβαση του ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας έχει ανασταλεί.
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731563"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>Υπέρβαση του ημερήσιου ορίου ηλεκτρονικού ταχυδρομείου. Η ροή εργασίας έχει ανασταλεί.

Αυτό το σφάλμα μπορεί να ληφθεί στα ακόλουθα σενάρια:

- Έχετε μια ροή εργασίας στο SharePoint Online που χρησιμοποιεί τον τύπο πλατφόρμας ροής εργασίας του SharePoint 2010 ή του SharePoint 2013.
- Η ροή εργασίας έχει ρυθμιστεί ώστε να στέλνει ένα προσαρμοσμένο μήνυμα ηλεκτρονικού ταχυδρομείου σε περισσότερους από 200 χρήστες κάθε φορά, περισσότερους από 10.000 παραλήπτες ανά ημέρα ή περισσότερα από 30 μηνύματα ανά λεπτό.
- Όταν εκτελείτε τη ροή εργασίας, το μήνυμα ηλεκτρονικού ταχυδρομείου δεν αποστέλλεται και παρατηρείτε την ακόλουθη συμπεριφορά:
    - Για μια ροή εργασίας που χρησιμοποιεί τον τύπο πλατφόρμας του SharePoint 2013, μεταβείτε στη σελίδα " **κατάσταση ροής εργασίας** ". Στη σελίδα "κατάσταση ροής εργασίας", η **εσωτερική κατάσταση** έχει τεθεί σε **Έναρξη**και το πλαίσιο πληροφοριών εμφανίζει τη **δυνατότητα αποστολής σε έναν παραλήπτη**.

Για να επιλύσετε αυτό το ζήτημα, ρυθμίστε τις παραμέτρους της ροής εργασίας για να στέλνετε μηνύματα ηλεκτρονικού ταχυδρομείου χωρίς να υπερβείτε τα [όρια αποστολέα του Exchange Online](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits). Για παράδειγμα, χρησιμοποιήστε μια παύση στη ροή εργασίας, στείλτε το μήνυμα ηλεκτρονικού ταχυδρομείου σε μια ομάδα του Microsoft 365, μια ομάδα διανομής ή μια ομάδα ασφαλείας με δυνατότητα αλληλογραφίας ή στείλτε το μήνυμα σε λιγότερους από 200 παραλήπτες κάθε φορά.


Για περισσότερες πληροφορίες, ανατρέξτε στο ακόλουθο [άρθρο](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or).

## <a name="related-topics"></a>Σχετικά θέματα
- [Δημιουργία ροής](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint και Flow](https://flow.microsoft.com/blog/sharepoint-and-flow/) 