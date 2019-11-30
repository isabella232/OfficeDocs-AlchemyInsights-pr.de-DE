---
title: Beheben von Office-Apps Sorry, wir haben eine temporäre Server Problemmeldung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: 4b90f843843416408d7f3091325fe436dc3ec9df
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627989"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="ec66f-102">Beheben der Office-Apps "Sorry, wir haben temporäre Server Probleme"-Nachricht</span><span class="sxs-lookup"><span data-stu-id="ec66f-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="ec66f-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="ec66f-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="ec66f-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="ec66f-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="ec66f-105">Siehe [Office 365 URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="ec66f-105">See [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="ec66f-106">Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein.</span><span class="sxs-lookup"><span data-stu-id="ec66f-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="ec66f-107">Stellen Sie sicher, dass die folgenden Dienste installiert sind:</span><span class="sxs-lookup"><span data-stu-id="ec66f-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="ec66f-108">Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet</span><span class="sxs-lookup"><span data-stu-id="ec66f-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="ec66f-109">Netzwerklisten Dienst</span><span class="sxs-lookup"><span data-stu-id="ec66f-109">Network List Service</span></span>
    - <span data-ttu-id="ec66f-110">Netzwerkstandort Erkennung</span><span class="sxs-lookup"><span data-stu-id="ec66f-110">Network Location Awareness</span></span>
    - <span data-ttu-id="ec66f-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="ec66f-111">Windows Event Log</span></span>

<span data-ttu-id="ec66f-112">Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="ec66f-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="ec66f-113">Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="ec66f-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="ec66f-114">**sfc-/scannow**</span><span class="sxs-lookup"><span data-stu-id="ec66f-114">**sfc /scannow**</span></span>

<span data-ttu-id="ec66f-115">Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="ec66f-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="ec66f-116">Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren von Office aus Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="ec66f-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate Office from Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>