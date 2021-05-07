---
title: „401 Nicht autorisiert“-Fehler in SharePoint
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
ms.openlocfilehash: 6799b2112458a7ab3715c9b63e03c2c7ca3fe6be
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233497"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="ef1b6-102">„401 Nicht autorisiert“-Fehler in SharePoint</span><span class="sxs-lookup"><span data-stu-id="ef1b6-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="ef1b6-p101">Wenn Sie in SharePoint die Fehlermeldung „(401) Nicht autorisiert“ erhalten, kann dies mit der veralteten TLS-Version 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="ef1b6-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

[<span data-ttu-id="ef1b6-105">Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="ef1b6-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

[<span data-ttu-id="ef1b6-106">Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat</span><span class="sxs-lookup"><span data-stu-id="ef1b6-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

<span data-ttu-id="ef1b6-107">Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.</span><span class="sxs-lookup"><span data-stu-id="ef1b6-107">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>