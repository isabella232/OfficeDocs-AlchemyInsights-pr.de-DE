---
title: Beheben 0x8004de40 Fehlers in OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649747"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a><span data-ttu-id="3af9a-102">Beheben 0x8004de40 Fehlers in OneDrive</span><span class="sxs-lookup"><span data-stu-id="3af9a-102">Fix 0x8004de40 error in OneDrive</span></span>

<span data-ttu-id="3af9a-103">Wenn Sie Windows 7 ausführen und diesen Fehler erhalten, aktualisieren Sie, um [TLS 1.1 und TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)als sichere Standardprotokolle in WinHTTP in Windows zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="3af9a-103">If you're running Windows 7 and receive this error, [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

<span data-ttu-id="3af9a-104">Wenn Sie Windows 10 ausführen und eine fehlermeldung 0x8004de40 OneDrive erhalten:</span><span class="sxs-lookup"><span data-stu-id="3af9a-104">If you're running Windows 10, and you receive an 0x8004de40 error with OneDrive:</span></span>

- <span data-ttu-id="3af9a-105">Starten Sie den betroffenen Computer neu, während er mit Ihrer Acitve Directory-Domäne verbunden ist.</span><span class="sxs-lookup"><span data-stu-id="3af9a-105">Reboot the affected computer while connected to your Acitve Directory domain.</span></span>
- <span data-ttu-id="3af9a-106">Wenn das Problem durch einen Neustart nicht behoben werden kann, müssen Sie dieJoinierung ihres Geräts von Azure AD aus wieder auf- und wieder durchführen.</span><span class="sxs-lookup"><span data-stu-id="3af9a-106">If a reboot doesn't fix the issue, unjoin and rejoin your device from Azure AD.</span></span> 

<span data-ttu-id="3af9a-107">**Hinweis:** Sie sollten sich in Ihrem Unternehmensnetzwerk befinden, während Sie diese Schritte ausführen.</span><span class="sxs-lookup"><span data-stu-id="3af9a-107">**Note**: You should be on your corporate network while performing these steps.</span></span> <span data-ttu-id="3af9a-108">Führen Sie diese Schritte nicht aus, wenn Sie nicht mit Ihrer Unternehmensinfrastruktur verbunden sind (z. B. unterwegs).</span><span class="sxs-lookup"><span data-stu-id="3af9a-108">Don't perform these steps when you aren't connected to your corporate infrastructure (for example, while traveling).</span></span> 

1. <span data-ttu-id="3af9a-109">Öffnen Sie eine Eingabeaufforderung mit erhöhten Rechten, indem Sie **Start** auswählen, klicken Sie mit der rechten Maustaste auf Eingabeaufforderung, und wählen Sie dann Als Administrator ausführen **aus.**</span><span class="sxs-lookup"><span data-stu-id="3af9a-109">Open an elevated command prompt by selecting **Start**, right-click **Command Prompt**, and then select **Run as administrator**.</span></span>

1. <span data-ttu-id="3af9a-110">Geben *Sie dsregcmd /leave ein, und* drücken Sie die **EINGABETASTE.**</span><span class="sxs-lookup"><span data-stu-id="3af9a-110">Type *dsregcmd /leave* and press **Enter**.</span></span>

1. <span data-ttu-id="3af9a-111">Geben Sie nach Abschluss *des Vorgangs dsregcmd /join ein, und drücken* Sie die **EINGABETASTE.**</span><span class="sxs-lookup"><span data-stu-id="3af9a-111">When complete, type *dsregcmd /join* and press **Enter**.</span></span>

1. <span data-ttu-id="3af9a-112">Schließen Sie nach Abschluss der Eingabeaufforderung die Eingabeaufforderung.</span><span class="sxs-lookup"><span data-stu-id="3af9a-112">When complete, close the command prompt.</span></span>

1. <span data-ttu-id="3af9a-113">Starten Sie den Computer neu, und melden Sie sich bei OneDrive an.</span><span class="sxs-lookup"><span data-stu-id="3af9a-113">Reboot the computer, and log into OneDrive.</span></span>