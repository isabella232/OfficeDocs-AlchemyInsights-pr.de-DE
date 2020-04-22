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
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764116"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a><span data-ttu-id="665fa-102">Beheben der Office-Apps "Sorry, wir haben temporäre Server Probleme"-Nachricht</span><span class="sxs-lookup"><span data-stu-id="665fa-102">Fixing the Office apps "Sorry, we are having temporary server issues" message</span></span>

<span data-ttu-id="665fa-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="665fa-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="665fa-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Office-Apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="665fa-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Office apps.</span></span> <span data-ttu-id="665fa-105">Siehe [URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="665fa-105">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

2. <span data-ttu-id="665fa-106">Wechseln Sie zu **Start** > **Ausführen**, und geben Sie **Services. msc**ein.</span><span class="sxs-lookup"><span data-stu-id="665fa-106">Go to **Start** > **Run**, and then type **services.msc**.</span></span> <span data-ttu-id="665fa-107">Stellen Sie sicher, dass die folgenden Dienste installiert sind:</span><span class="sxs-lookup"><span data-stu-id="665fa-107">Make sure that the following services are all running:</span></span>
    - <span data-ttu-id="665fa-108">Mit dem Netzwerk verbundene Geräte werden automatisch eingerichtet</span><span class="sxs-lookup"><span data-stu-id="665fa-108">Network Connected Devices Auto-Setup</span></span>
    - <span data-ttu-id="665fa-109">Netzwerklisten Dienst</span><span class="sxs-lookup"><span data-stu-id="665fa-109">Network List Service</span></span>
    - <span data-ttu-id="665fa-110">Netzwerkstandort Erkennung</span><span class="sxs-lookup"><span data-stu-id="665fa-110">Network Location Awareness</span></span>
    - <span data-ttu-id="665fa-111">Windows-Ereignisprotokoll</span><span class="sxs-lookup"><span data-stu-id="665fa-111">Windows Event Log</span></span>

<span data-ttu-id="665fa-112">Wenn einer dieser Dienste nicht aktiv ist, versuchen Sie, ihn zu starten.</span><span class="sxs-lookup"><span data-stu-id="665fa-112">If one of these services is not running, try to start it.</span></span> <span data-ttu-id="665fa-113">Wenn beim Starten des Diensts ein Problem auftritt, führen Sie den folgenden Befehl aus, indem Sie eine Eingabeaufforderung mit erhöhten Berechtigungen öffnen:</span><span class="sxs-lookup"><span data-stu-id="665fa-113">If you have a problem starting the service, run the following command by opening a command prompt with elevated permissions:</span></span>

<span data-ttu-id="665fa-114">**sfc-/scannow**</span><span class="sxs-lookup"><span data-stu-id="665fa-114">**sfc /scannow**</span></span>

<span data-ttu-id="665fa-115">Nachdem dieser Befehl abgeschlossen ist, starten Sie den Computer neu.</span><span class="sxs-lookup"><span data-stu-id="665fa-115">After this command finishes, restart the computer.</span></span>

<span data-ttu-id="665fa-116">Ausführliche Informationen finden Sie unter ["Sorry, wir können keine Verbindung zu Ihrem Konto herstellen. Versuchen Sie es später erneut "Fehler beim Aktivieren](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span><span class="sxs-lookup"><span data-stu-id="665fa-116">For detailed information, see ["Sorry, we can't connect to your account. Please try again later" error when you activate](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).</span></span>