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
ms.openlocfilehash: ac2fe27a8e7b277bfaf18303bf5b792410a1ea6a
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539931"
---
# <a name="401-unauthorized-error-in-sharepoint"></a><span data-ttu-id="b748c-102">„401 Nicht autorisiert“-Fehler in SharePoint</span><span class="sxs-lookup"><span data-stu-id="b748c-102">401 Unauthorized error in SharePoint</span></span>

<span data-ttu-id="b748c-p101">Wenn Sie in SharePoint die Fehlermeldung „(401) Nicht autorisiert“ erhalten, kann dies mit der veralteten TLS-Version 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="b748c-p101">If you receive the error "(401) Unauthorized" in SharePoint it might be related to the deprecation of TLS 1.0/1.1. For more info, see:</span></span>

- [<span data-ttu-id="b748c-105">Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC</span><span class="sxs-lookup"><span data-stu-id="b748c-105">Preparing for TLS 1.2 in Office 365 and Office 365 GCC</span></span>](/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [<span data-ttu-id="b748c-106">Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat</span><span class="sxs-lookup"><span data-stu-id="b748c-106">Authentication errors occur if client doesn't have TLS 1.2 support</span></span>](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [<span data-ttu-id="b748c-107">Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows</span><span class="sxs-lookup"><span data-stu-id="b748c-107">Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows</span></span>](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

<span data-ttu-id="b748c-108">Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.</span><span class="sxs-lookup"><span data-stu-id="b748c-108">If users are on Windows 7, make sure they check [TLS Cipher Suites in Windows 7](/windows/win32/secauthn/tls-cipher-suites-in-windows-7).</span></span>