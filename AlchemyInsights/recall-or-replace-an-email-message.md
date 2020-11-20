---
title: Rückruf oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1860"
- "9000260"
ms.assetid: ''
ms.openlocfilehash: 05016213a1387c5290cb5899359f1f10b5a413c0
ms.sourcegitcommit: 4e0ae808ee2a586339b396320e3edb8ba066a91a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/19/2020
ms.locfileid: "49353505"
---
# <a name="recall-or-replace-an-email-message-in-microsoft-365"></a><span data-ttu-id="e7655-102">Rückruf oder Ersetzen einer e-Mail-Nachricht in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="e7655-102">Recall or replace an email message in Microsoft 365</span></span>

- <span data-ttu-id="e7655-103">Sie können **nur Nachrichten abrufen, die an Personen in Ihrer Organisation gesendet werden**.</span><span class="sxs-lookup"><span data-stu-id="e7655-103">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="e7655-104">Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr abrufen.</span><span class="sxs-lookup"><span data-stu-id="e7655-104">For example, if the message was sent to a Gmail address, you can't recall it.</span></span>
- <span data-ttu-id="e7655-105">Sie können **nur Nachrichten abrufen, die von Outlook für den PC gesendet wurden**.</span><span class="sxs-lookup"><span data-stu-id="e7655-105">You can **only recall messages sent from Outlook for the PC**.</span></span> <span data-ttu-id="e7655-106">Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Internet sendet, kann er nicht mehr daran erinnert werden.</span><span class="sxs-lookup"><span data-stu-id="e7655-106">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>
- <span data-ttu-id="e7655-107">Als mandantenadministrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen** (Weitere Informationen finden Sie unter: [Suchen nach und Löschen von e-Mail-Nachrichten](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span><span class="sxs-lookup"><span data-stu-id="e7655-107">As a tenant administrator, you can **recall messages on behalf of users by using PowerShell** (For more information, see: [Search for and delete email messages](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messages-in-your-organization)).</span></span>
- <span data-ttu-id="e7655-108">Sie können keine Nachrichten aus dem Admin Center abrufen.</span><span class="sxs-lookup"><span data-stu-id="e7655-108">You can't recall messages from the admin center.</span></span> <span data-ttu-id="e7655-109">Scrollen Sie nach unten zu "suchen und Löschen von e-Mail-Nachrichten in Ihrer Organisation", um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="e7655-109">Scroll down to "Search for and delete email messages in your organization" for more information.</span></span>

<span data-ttu-id="e7655-110">**Zurückrufen oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht**</span><span class="sxs-lookup"><span data-stu-id="e7655-110">**Recall or replace an email message that you sent**</span></span>

1. <span data-ttu-id="e7655-111">Wählen Sie im Bereich Ordner auf der linken Seite des Outlook-Fensters den Ordner Gesendete Elemente aus.</span><span class="sxs-lookup"><span data-stu-id="e7655-111">In the folder pane on the left of the Outlook window, choose the Sent Items folder.</span></span>
2. <span data-ttu-id="e7655-112">Öffnen Sie die Nachricht, die Sie abrufen möchten.</span><span class="sxs-lookup"><span data-stu-id="e7655-112">Open the message that you want to recall.</span></span> <span data-ttu-id="e7655-113">Sie müssen doppelklicken, um die Nachricht zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="e7655-113">You must double-click to open the message.</span></span> <span data-ttu-id="e7655-114">Wenn Sie die Nachricht auswählen, damit Sie im Lesebereich angezeigt wird, können Sie die Nachricht nicht mehr abrufen.</span><span class="sxs-lookup"><span data-stu-id="e7655-114">Selecting the message so it appears in the reading pane won't allow you to recall the message.</span></span>
3. <span data-ttu-id="e7655-115">Wählen Sie auf der Registerkarte Nachricht die Option **Aktionen**  >  **Rückruf dieser Nachricht** aus.</span><span class="sxs-lookup"><span data-stu-id="e7655-115">From the Message tab, select **Actions** > **Recall This Message**.</span></span>
4. <span data-ttu-id="e7655-116">Wählen Sie **Ungelesene Kopien dieser Nachricht löschen** oder **Ungelesene Kopien löschen aus, und ersetzen Sie Sie durch eine neue Nachricht, und** wählen Sie dann **OK** aus.</span><span class="sxs-lookup"><span data-stu-id="e7655-116">Choose **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, then select **OK**.</span></span>
5. <span data-ttu-id="e7655-117">Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden** aus.</span><span class="sxs-lookup"><span data-stu-id="e7655-117">If you're sending a replacement message, compose the message, then select **Send**.</span></span>
6. <span data-ttu-id="e7655-118">Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen der Empfänger in Outlook ab.</span><span class="sxs-lookup"><span data-stu-id="e7655-118">The success or failure of a message recall depends on the recipients' settings in Outlook.</span></span>

<span data-ttu-id="e7655-119">Weitere Informationen, einschließlich der Vorgehensweise zum Überprüfen des Rückrufs, finden Sie unter [Rückruf oder Ersetzen einer von Ihnen gesendeten e-Mail-Nachricht](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="e7655-119">For more information, including how to check on the recall, see [Recall or replace an email message that you sent](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="e7655-120">**_Zum Suchen nach und Löschen von e-Mail-Nachrichten in Ihrer Organisation_** ist es am einfachsten, wenn Sie ein globaler Administrator sind. Wenn Sie kein globaler Administrator sind, muss Ihr Konto der Rollengruppe "eDiscovery-Manager" oder der Rolle "Compliance Search Management" hinzugefügt werden.</span><span class="sxs-lookup"><span data-stu-id="e7655-120">**_To search for and delete email messages in your organization_**, it's easiest if you're a global admin. If you're not a global admin, your account must be added to the eDiscovery Manager role group, or to the Compliance Search management role.</span></span> <span data-ttu-id="e7655-121">Wenn Sie Nachrichten löschen möchten, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Rolle "Such-und Lösch Verwaltung" beitreten.</span><span class="sxs-lookup"><span data-stu-id="e7655-121">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="e7655-122">Berechtigungen für diese Rollen werden im [Security & Compliance Center](https://protection.office.com/)zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="e7655-122">Permissions to these roles are assigned in the [Security & compliance center](https://protection.office.com/).</span></span>

1. <span data-ttu-id="e7655-123">[Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu suchen.</span><span class="sxs-lookup"><span data-stu-id="e7655-123">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
2. <span data-ttu-id="e7655-124">[Stellen Sie eine Verbindung mit der Security & Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="e7655-124">[Connect to Security & Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell).</span></span>

<span data-ttu-id="e7655-125">Wenn Sie MFA (Multi-Factor Authentication) verwenden, finden Sie unter [Connect to Microsoft 365 Security & Compliance Center PowerShell mit mehr](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell)stufiger Authentifizierung.</span><span class="sxs-lookup"><span data-stu-id="e7655-125">If you're using MFA (multi-factor authentication), see [Connect to Microsoft 365 Security & Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell).</span></span>
