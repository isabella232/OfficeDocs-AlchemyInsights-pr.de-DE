---
title: Hängen im Postausgang aufgrund großer Anlagen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232629"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="e5fd7-102">Beheben von Nachrichten, die im Postausgang hängen</span><span class="sxs-lookup"><span data-stu-id="e5fd7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="e5fd7-103">Es wird empfohlen, dass Sie zunächst das Szenario ["Ich habe Probleme beim Senden, empfangen oder finden von e-Mail-Nachrichten"](https://aka.ms/SaRA-OutlookSendReceive) vom [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) -Tool auf dem betroffenen Computer aus starten.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="e5fd7-104">Wenn eine Nachricht in Ihrem Postausgang feststeht, ist die wahrscheinlichste Ursache eine große Anlage oder die Option "sofort bei Verbindung senden" ist nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="e5fd7-105">**Entfernen der großen Anlage**</span><span class="sxs-lookup"><span data-stu-id="e5fd7-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="e5fd7-106">Klicken Sie auf **senden/empfangen** > **Arbeiten offline**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="e5fd7-107">Klicken Sie im Navigationsbereich auf **Postausgang**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="e5fd7-108">Von hier aus haben Sie folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="e5fd7-108">From here, you can:</span></span> 
    - <span data-ttu-id="e5fd7-109">Löschen Sie die Nachricht.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-109">Delete the message.</span></span> <span data-ttu-id="e5fd7-110">Wählen Sie Sie einfach aus, und klicken Sie auf **Löschen**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="e5fd7-111">Ziehen Sie die Nachricht in den **Ordner Entwürfe**, doppelklicken Sie auf, um die Nachricht zu öffnen, und löschen Sie die Anlage (Klicken Sie darauf, und klicken Sie auf **Löschen**).</span><span class="sxs-lookup"><span data-stu-id="e5fd7-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="e5fd7-112">Wenn ein Fehler besagt, dass Outlook versucht, die Nachricht zu übermitteln, schließen Sie Outlook.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="e5fd7-113">Es kann ein paar Augenblicke dauern, bis das Programm beendet ist.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-113">It may take a few moments to exit.</span></span> <span data-ttu-id="e5fd7-114">Wenn Outlook nicht geschlossen wird, drücken Sie **STRG + ALT + ENTF** , und klicken Sie auf **Task-Manager starten**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="e5fd7-115">Wählen Sie im Task-Manager die Registerkarte **Prozesse** aus, Scrollen Sie nach unten zu Outlook. exe, und klicken Sie dann auf **Prozess beenden**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="e5fd7-116">Nachdem Outlook geschlossen wurde, starten Sie Outlook neu, und wiederholen Sie die Schritte 2-3.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="e5fd7-117">Nachdem Sie die Anlage entfernt haben, klicken Sie auf **senden/empfangen** > **Arbeiten offline** , um die Auswahl der Schaltfläche aufzuheben und die Online Arbeit fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="e5fd7-118">Nachrichten werden auch im Postausgang festgehalten, wenn Sie auf **senden**klicken, aber keine Verbindung hergestellt ist.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="e5fd7-119">Klicken Sie auf **senden/empfangen** und sehen Sie sich die Schaltfläche **Offline arbeiten** an.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="e5fd7-120">Wenn es blau ist, sind Sie getrennt.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="e5fd7-121">Klicken Sie darauf, um eine Verbindung herzustellen (die Schaltfläche wird weiß), und klicken Sie auf **Alle senden**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="e5fd7-122">**Sofortnachrichten senden bei Verbindung aktivieren**</span><span class="sxs-lookup"><span data-stu-id="e5fd7-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="e5fd7-123">Klicken Sie auf der Registerkarte Datei auf **Optionen**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="e5fd7-124">Klicken Sie im Dialogfeld Outlook-Optionen auf **erweitert**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="e5fd7-125">Klicken Sie im Abschnitt senden und empfangen auf, um **bei einer Verbindung sofort senden**zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="e5fd7-126">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="e5fd7-126">Click **OK**.</span></span>
 
<span data-ttu-id="e5fd7-127">Ausführliche Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="e5fd7-127">For full details, see:</span></span>
- [<span data-ttu-id="e5fd7-128">Video: senden oder Löschen einer Stuck-e-Mail</span><span class="sxs-lookup"><span data-stu-id="e5fd7-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="e5fd7-129">E-Mail-Nachrichten bleiben im Ordner Postausgang, bis Sie einen Sende-oder Empfangsvorgang in Outlook manuell initiieren</span><span class="sxs-lookup"><span data-stu-id="e5fd7-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
