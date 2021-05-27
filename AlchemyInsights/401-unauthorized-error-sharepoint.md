---
title: 401 Μη εξουσιοδοτημένο σφάλμα στο SharePoint
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10935"
- "9001435"
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: el-GR
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539932"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="89773-102">401 Μη εξουσιοδοτημένο σφάλμα στο SharePoint</span><span class="sxs-lookup"><span data-stu-id="89773-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="89773-103">Εάν εμφανιστεί το σφάλμα "(401) Μη εξουσιοδοτημένη" στο SharePoint μπορεί να σχετίζεται με την κατάργηση του TLS 1.0/1.1.</span><span class="sxs-lookup"><span data-stu-id="89773-103">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1.</span></span> <span data-ttu-id="89773-104">Για περισσότερες πληροφορίες, ανατρέξτε στα παρακάτω θέματα:</span><span class="sxs-lookup"><span data-stu-id="89773-104">For more info, see:</span></span>

- [<span data-ttu-id="89773-105">Προετοιμασία για TLS 1.2 σε Office 365 και Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="89773-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="89773-106">Σφάλματα ελέγχου ταυτότητας προκύπτουν εάν το πρόγραμμα-πελάτης δεν έχει υποστήριξη TLS 1.2</span><span class="sxs-lookup"><span data-stu-id="89773-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="89773-107">Ενημέρωση για την ενεργοποίηση των TLS 1.1 και TLS 1.2 ως προεπιλεγμένων ασφαλών πρωτοκόλλων στο WinHTTP στο Windows</span><span class="sxs-lookup"><span data-stu-id="89773-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="89773-108">Εάν οι χρήστες βρίσκονται στο Windows 7, βεβαιωθείτε ότι ελέγχουν τις οικογένειες προγραμμάτων [κρυπτογράφησης TLS στο Windows 7.](/windows/win32/secauthn/tls-cipher-suites-in-windows-7)</span><span class="sxs-lookup"><span data-stu-id="89773-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>