---
title: Aktivierungsproblem – jetzt können wir keine Verbindung herstellen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725982"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a><span data-ttu-id="fad38-102">Beheben der Microsoft 365-Apps "Wir können die Verbindung jetzt nicht herstellen"-Nachricht</span><span class="sxs-lookup"><span data-stu-id="fad38-102">Fixing the Microsoft 365 apps "We are unable to connect right now" message</span></span>

<span data-ttu-id="fad38-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="fad38-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="fad38-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Microsoft 365-apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="fad38-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="fad38-105">Siehe [Microsoft-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="fad38-105">See [Microsoft URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="fad38-106">Wechseln Sie zu **Start**  >  **Ausführen**, und geben Sie **Services. msc**ein.</span><span class="sxs-lookup"><span data-stu-id="fad38-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="fad38-107">Stellen Sie sicher, dass die folgenden Dienste installiert sind:</span><span class="sxs-lookup"><span data-stu-id="fad38-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="fad38-108">Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet</span><span class="sxs-lookup"><span data-stu-id="fad38-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="fad38-109">Netzwerklisten Dienst</span><span class="sxs-lookup"><span data-stu-id="fad38-109">Network List Service</span></span>
    - <span data-ttu-id="fad38-110">Netzwerkstandort Erkennung</span><span class="sxs-lookup"><span data-stu-id="fad38-110">Network Location Awareness</span></span>
    - <span data-ttu-id="fad38-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="fad38-111">Windows Event Log</span></span>

<span data-ttu-id="fad38-112">Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="fad38-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="fad38-113">Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="fad38-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="fad38-114">**sfc-/scannow**</span><span class="sxs-lookup"><span data-stu-id="fad38-114">**sfc /scannow**</span></span>

<span data-ttu-id="fad38-115">Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="fad38-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="fad38-116">Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office von Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="fad38-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>