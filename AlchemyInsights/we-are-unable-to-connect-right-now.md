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
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716171"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="6d297-102">Beheben der Office-Apps "Wir können jetzt keine Verbindung herstellen"-Nachricht</span><span class="sxs-lookup"><span data-stu-id="6d297-102">Fixing the Office apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="6d297-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="6d297-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6d297-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="6d297-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="6d297-105">Siehe [Microsoft-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6d297-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="6d297-106">Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein.</span><span class="sxs-lookup"><span data-stu-id="6d297-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="6d297-107">Stellen Sie sicher, dass die folgenden Dienste installiert sind:</span><span class="sxs-lookup"><span data-stu-id="6d297-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="6d297-108">Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet</span><span class="sxs-lookup"><span data-stu-id="6d297-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="6d297-109">Netzwerklisten Dienst</span><span class="sxs-lookup"><span data-stu-id="6d297-109">Network List Service</span></span>
    - <span data-ttu-id="6d297-110">Netzwerkstandort Erkennung</span><span class="sxs-lookup"><span data-stu-id="6d297-110">Network Location Awareness</span></span>
    - <span data-ttu-id="6d297-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="6d297-111">Windows Event Log</span></span>

<span data-ttu-id="6d297-112">Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="6d297-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="6d297-113">Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="6d297-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="6d297-114">**sfc-/scannow**</span><span class="sxs-lookup"><span data-stu-id="6d297-114">**sfc /scannow**</span></span>

<span data-ttu-id="6d297-115">Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="6d297-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="6d297-116">Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office von Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="6d297-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>