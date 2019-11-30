---
title: Aktivierungsproblem – jetzt können wir keine Verbindung herstellen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628241"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="f7002-102">Beheben der Office-Apps "Wir können jetzt keine Verbindung herstellen"-Nachricht</span><span class="sxs-lookup"><span data-stu-id="f7002-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="f7002-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="f7002-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="f7002-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="f7002-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="f7002-105">Siehe [Office 365 URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="f7002-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="f7002-106">Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein.</span><span class="sxs-lookup"><span data-stu-id="f7002-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="f7002-107">Stellen Sie sicher, dass die folgenden Dienste installiert sind:</span><span class="sxs-lookup"><span data-stu-id="f7002-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="f7002-108">Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet</span><span class="sxs-lookup"><span data-stu-id="f7002-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="f7002-109">Netzwerklisten Dienst</span><span class="sxs-lookup"><span data-stu-id="f7002-109">Network List Service</span></span>
    - <span data-ttu-id="f7002-110">Netzwerkstandort Erkennung</span><span class="sxs-lookup"><span data-stu-id="f7002-110">Network Location Awareness</span></span>
    - <span data-ttu-id="f7002-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="f7002-111">Windows Event Log</span></span>

<span data-ttu-id="f7002-112">Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="f7002-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="f7002-113">Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="f7002-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="f7002-114">**sfc-/scannow**</span><span class="sxs-lookup"><span data-stu-id="f7002-114">**sfc /scannow**</span></span>

<span data-ttu-id="f7002-115">Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="f7002-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="f7002-116">Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office aus Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="f7002-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>