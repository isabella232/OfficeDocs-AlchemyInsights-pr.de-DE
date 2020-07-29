---
title: Verwenden von TeamViewer für die Remoteverwaltung von Intune-Geräten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505210"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="5507f-102">Verwenden von TeamViewer für die Remoteverwaltung von Intune-Geräten</span><span class="sxs-lookup"><span data-stu-id="5507f-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="5507f-103">Von Intune verwaltete Geräte können mithilfe von [TeamViewer](https://www.teamviewer.com/) remote verwaltet werden.</span><span class="sxs-lookup"><span data-stu-id="5507f-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="5507f-104">Führen Sie die folgenden Schritte aus, um Intune mithilfe von TeamViewer zu verwalten:</span><span class="sxs-lookup"><span data-stu-id="5507f-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="5507f-105">Beginnen Sie damit, dass Sie Anmeldeinformationen von TeamViewer abrufen, um den TeamViewer-Connector in Intune einzurichten.</span><span class="sxs-lookup"><span data-stu-id="5507f-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="5507f-106">Auf diese Weise kann der Administrator Anmeldeinformationen in der Benutzeroberfläche des TeamViewer-Connectors unter „Geräte“ eingeben. Hierbei handelt es sich um einen einmaligen Vorgang zum Herstellen der Verknüpfung zwischen Intune und dem TeamViewer-Dienst.</span><span class="sxs-lookup"><span data-stu-id="5507f-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="5507f-107">**Teil 1: Starten einer Sitzung mit einem Remotegerät**</span><span class="sxs-lookup"><span data-stu-id="5507f-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="5507f-108">Wählen Sie unter **Alle Geräte** das Gerät aus, mit dem Sie eine Remotesitzung starten möchten.</span><span class="sxs-lookup"><span data-stu-id="5507f-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="5507f-109">Wählen Sie unter **...Mehr** die Option **Neue Remoteunterstützungssitzung** aus.</span><span class="sxs-lookup"><span data-stu-id="5507f-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="5507f-110">Wählen Sie **Ja** aus, um zu bestätigen, dass Sie eine Remotesitzung einrichten möchten.</span><span class="sxs-lookup"><span data-stu-id="5507f-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="5507f-111">Nachdem die Anforderung zur „Initiierung einer neuen Remotesitzung“ vom TeamViewer-Dienst bestätigt wurde, wird unter den Details des Bereichs „Übersicht“ (oder „Essentials“) für das Gerät eine Option **Remotesitzung starten** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="5507f-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="5507f-112">Wählen Sie **Mehr anzeigen** aus, um den Bereich zu erweitern und den Status der Remoteunterstützung anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="5507f-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="5507f-113">Wählen Sie **Remotesitzung starten** aus, um die Sitzung auf der Administratorseite zu initiieren.</span><span class="sxs-lookup"><span data-stu-id="5507f-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="5507f-114">Wählen Sie das Herunterladen der TeamViewer-Binärdatei (Windows) aus, und wählen Sie **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="5507f-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="5507f-115">**Hinweis**: Sie können alle Webbrowserseiten ignorieren, die auf der TeamViewer-Website geöffnet sind.</span><span class="sxs-lookup"><span data-stu-id="5507f-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="5507f-116">Bestätigen Sie die Anforderung der TeamViewer-App zur Vornahme von Änderungen an dem Gerät (nur Windows).</span><span class="sxs-lookup"><span data-stu-id="5507f-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="5507f-117">Die TeamViewer-App wird gestartet und enthält den Sitzungscode, um die Verbindung mit dem Remotegerät zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="5507f-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="5507f-118">**Teil 2: Auf dem Gerät, das das Ziel einer Remotesitzung ist**</span><span class="sxs-lookup"><span data-stu-id="5507f-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="5507f-119">Öffnen Sie das Intune-Unternehmensportal.</span><span class="sxs-lookup"><span data-stu-id="5507f-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="5507f-120">Suchen Sie nach einer Benachrichtigungskennzeichnung: „Ihr IT-Administrator fordert die Kontrolle über dieses Geräts für eine Remoteunterstützungssitzung an“, und wählen Sie die Benachrichtigung aus.</span><span class="sxs-lookup"><span data-stu-id="5507f-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="5507f-121">Wählen Sie das Herunterladen der TeamViewer-Anwendung aus, oder bestätigen Sie den Download der TeamViewer-App aus dem App Store, und wählen Sie **Ausführen** aus.</span><span class="sxs-lookup"><span data-stu-id="5507f-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="5507f-122">**Hinweis**: Sie können alle Webbrowserseiten ignorieren, die auf der TeamViewer-Website geöffnet sind.</span><span class="sxs-lookup"><span data-stu-id="5507f-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="5507f-123">Bestätigen Sie die Anforderung der TeamViewer-App zur Vornahme von Änderungen an dem Gerät (nur Windows).</span><span class="sxs-lookup"><span data-stu-id="5507f-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="5507f-124">Die TeamViewer-App wird gestartet und enthält den Sitzungscode, um die Verbindung mit dem Remotegerät zu authentifizieren.</span><span class="sxs-lookup"><span data-stu-id="5507f-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="5507f-125">In einem Popup werden Sie gefragt, ob Sie den Start der Sitzung zulassen möchten.</span><span class="sxs-lookup"><span data-stu-id="5507f-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="5507f-126">**Hinweis**: Die vom TeamViewer-Dienst generierten Sitzungscodes können nur einmalig verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="5507f-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="5507f-127">Wenn die Verbindung getrennt wird, müssen Sie:</span><span class="sxs-lookup"><span data-stu-id="5507f-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="5507f-128">Die Instanz der TeamViewer-App auf dem Remotegerät und auf der Administratorarbeitsstation schließen.</span><span class="sxs-lookup"><span data-stu-id="5507f-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="5507f-129">Das Unternehmensportal auf dem Remotegerät schließen.</span><span class="sxs-lookup"><span data-stu-id="5507f-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="5507f-130">Eine „Neue Remoteunterstützungssitzung“ aus dem Verwaltungsportal initiieren.</span><span class="sxs-lookup"><span data-stu-id="5507f-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="5507f-131">Das Unternehmensportal auf dem Remotegerät erneut öffnen, um die neue Benachrichtigung zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="5507f-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="5507f-132">Die TeamViewer-App herunterladen und wie zuvor sowohl auf dem Remotegerät als auch auf der Administratorarbeitsstation öffnen.</span><span class="sxs-lookup"><span data-stu-id="5507f-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>