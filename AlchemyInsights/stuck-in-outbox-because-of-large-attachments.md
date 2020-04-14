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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241251"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="130d7-102">Beheben von Nachrichten, die im Postausgang hängen</span><span class="sxs-lookup"><span data-stu-id="130d7-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="130d7-103">Es wird empfohlen, dass Sie zunächst das Szenario ["Ich habe Probleme beim Senden, empfangen oder finden von e-Mail-Nachrichten"](https://aka.ms/SaRA-OutlookSendReceive) im [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) -Tool durchführen.</span><span class="sxs-lookup"><span data-stu-id="130d7-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="130d7-104">Wenn eine Nachricht in Ihrem Postausgang feststeht, ist die wahrscheinlichste Ursache eine große Anlage oder die Option "sofort bei Verbindung senden" ist nicht aktiviert.</span><span class="sxs-lookup"><span data-stu-id="130d7-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="130d7-105">**Entfernen der großen Anlage**</span><span class="sxs-lookup"><span data-stu-id="130d7-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="130d7-106">Wählen Sie in Outlook **senden/empfangen** > **Arbeiten offline**aus.</span><span class="sxs-lookup"><span data-stu-id="130d7-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="130d7-107">Wählen Sie im Navigationsbereich die Option **Postausgang**aus.</span><span class="sxs-lookup"><span data-stu-id="130d7-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="130d7-108">Von hier aus haben Sie folgende Möglichkeiten:</span><span class="sxs-lookup"><span data-stu-id="130d7-108">From here, you can:</span></span> 
    - <span data-ttu-id="130d7-109">Löschen Sie die Nachricht (Wählen Sie Sie aus, und wählen Sie dann **Löschen**aus).</span><span class="sxs-lookup"><span data-stu-id="130d7-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="130d7-110">Ziehen Sie die Nachricht in den Ordner Entwürfe, doppelklicken Sie darauf, um Sie zu öffnen, und entfernen Sie die Anlage, wählen Sie Sie aus, und wählen Sie dann **Löschen**aus.</span><span class="sxs-lookup"><span data-stu-id="130d7-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="130d7-111">Wenn Sie eine Fehlermeldung erhalten, die besagt, dass Outlook versucht, die Nachricht zu übermitteln, schließen Sie Outlook.</span><span class="sxs-lookup"><span data-stu-id="130d7-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="130d7-112">Es kann ein paar Augenblicke dauern, bis das Programm beendet ist.</span><span class="sxs-lookup"><span data-stu-id="130d7-112">It may take a few moments to exit.</span></span> <span data-ttu-id="130d7-113">Wenn Outlook nicht geschlossen wird, drücken Sie STRG + ALT + ENTF, und klicken Sie dann auf **Task-Manager starten**.</span><span class="sxs-lookup"><span data-stu-id="130d7-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="130d7-114">Wählen Sie im Task-Manager die Registerkarte **Prozesse** aus, Scrollen Sie nach unten zu Outlook. exe, und wählen Sie **Prozess beenden**aus.</span><span class="sxs-lookup"><span data-stu-id="130d7-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="130d7-115">Nachdem Outlook geschlossen wurde, starten Sie es neu, und wiederholen Sie die Schritte 2 und 3.</span><span class="sxs-lookup"><span data-stu-id="130d7-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="130d7-116">Nachdem Sie die Anlage entfernt haben, klicken Sie auf **senden/empfangen** > **Arbeiten offline** , um die Online Arbeit fortzusetzen.</span><span class="sxs-lookup"><span data-stu-id="130d7-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="130d7-117">Nachrichten werden auch im Postausgang festgehalten, wenn Sie auf **senden**klicken, aber keine Verbindung hergestellt ist.</span><span class="sxs-lookup"><span data-stu-id="130d7-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="130d7-118">Klicken Sie auf **senden/empfangen** und sehen Sie sich die Schaltfläche **Offline arbeiten** an.</span><span class="sxs-lookup"><span data-stu-id="130d7-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="130d7-119">Wenn es blau ist, sind Sie getrennt.</span><span class="sxs-lookup"><span data-stu-id="130d7-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="130d7-120">Klicken Sie darauf, um eine Verbindung herzustellen (die Schaltfläche wird weiß), und klicken Sie auf **Alle senden**.</span><span class="sxs-lookup"><span data-stu-id="130d7-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="130d7-121">**Sofortnachrichten senden bei Verbindung aktivieren**</span><span class="sxs-lookup"><span data-stu-id="130d7-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="130d7-122">Klicken Sie auf der Registerkarte Datei auf **Optionen**.</span><span class="sxs-lookup"><span data-stu-id="130d7-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="130d7-123">Klicken Sie im Dialogfeld Outlook-Optionen auf **erweitert**.</span><span class="sxs-lookup"><span data-stu-id="130d7-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="130d7-124">Klicken Sie im Abschnitt senden und empfangen auf, um **bei einer Verbindung sofort senden**zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="130d7-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="130d7-125">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="130d7-125">Click **OK**.</span></span>
 
<span data-ttu-id="130d7-126">Ausführliche Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="130d7-126">For full details, see:</span></span>
- [<span data-ttu-id="130d7-127">Video: senden oder Löschen einer Stuck-e-Mail</span><span class="sxs-lookup"><span data-stu-id="130d7-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="130d7-128">E-Mail-Nachrichten bleiben im Ordner Postausgang, bis Sie einen Sende-oder Empfangsvorgang in Outlook manuell initiieren</span><span class="sxs-lookup"><span data-stu-id="130d7-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
