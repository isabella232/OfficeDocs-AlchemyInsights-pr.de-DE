---
title: Beheben von Microsoft 365-Apps Leider gibt es eine Meldung zu temporären Serverproblemen
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 0adf1d66869051b9dd8290ef3466ef9b13aa2d41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51835270"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="49958-102">Beheben der Microsoft 365-Apps "Leider haben wir temporäre Serverprobleme"</span><span class="sxs-lookup"><span data-stu-id="49958-102">Fixing the Microsoft 365 apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="49958-103">Wenn Sie diese Nachricht erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="49958-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="49958-104">Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um zu überprüfen, ob sie den Internetzugriff auf Microsoft 365-Apps nicht blockieren.</span><span class="sxs-lookup"><span data-stu-id="49958-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="49958-105">Weitere [Informationen finden Sie unter URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="49958-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="49958-106">Wechseln Sie **zu Start**  >  **Ausführen**, und geben Sie **dann services.msc ein.**</span><span class="sxs-lookup"><span data-stu-id="49958-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="49958-107">Stellen Sie sicher, dass die folgenden Dienste ausgeführt werden:</span><span class="sxs-lookup"><span data-stu-id="49958-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="49958-108">Automatisches Einrichten von netzwerkgebundenen Geräten</span><span class="sxs-lookup"><span data-stu-id="49958-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="49958-109">Netzwerklistendienst</span><span class="sxs-lookup"><span data-stu-id="49958-109">Network List Service</span></span>
    - <span data-ttu-id="49958-110">Netzwerkstandortbewusstsein</span><span class="sxs-lookup"><span data-stu-id="49958-110">Network Location Awareness</span></span>
    - <span data-ttu-id="49958-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="49958-111">Windows Event Log</span></span>

<span data-ttu-id="49958-112">Wenn einer dieser Dienste nicht ausgeführt wird, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="49958-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="49958-113">Wenn beim Starten des Diensts ein Problem besteht, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="49958-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="49958-114">**sfc /scannow**</span><span class="sxs-lookup"><span data-stu-id="49958-114">**sfc /scannow**</span></span>

<span data-ttu-id="49958-115">Starten Sie nach Abschluss dieses Befehls den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="49958-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="49958-116">Ausführliche Informationen finden Sie unter "Leider können [wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es später erneut"-Fehler, wenn Sie aktivieren.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)</span><span class="sxs-lookup"><span data-stu-id="49958-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>