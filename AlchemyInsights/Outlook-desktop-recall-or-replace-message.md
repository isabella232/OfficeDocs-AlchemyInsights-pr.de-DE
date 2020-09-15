---
title: Outlook-Desktop Rückruf oder Ersetzen einer e-Mail-Nachricht
ms.author: daeite
author: daeite
manager: joallard
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.custom: 9000260
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.openlocfilehash: 578e2690061286bde74ee0b4b74a197630716f59
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663989"
---
# <a name="recall-or-replace-an-outlook-email-message"></a><span data-ttu-id="62f17-102">Rückruf oder Ersetzen einer Outlook-e-Mail-Nachricht</span><span class="sxs-lookup"><span data-stu-id="62f17-102">Recall or replace an Outlook email message</span></span>

- <span data-ttu-id="62f17-103">Als Administrator können Sie **Nachrichten im Namen von Benutzern mithilfe von PowerShell abrufen**.</span><span class="sxs-lookup"><span data-stu-id="62f17-103">As the admin, you can **recall messages on behalf of users using PowerShell**.</span></span> <span data-ttu-id="62f17-104">Sie können keine Nachrichten aus dem Admin Center abrufen.</span><span class="sxs-lookup"><span data-stu-id="62f17-104">You can't recall messages from the admin center.</span></span>
- <span data-ttu-id="62f17-105">Sie können **nur Nachrichten abrufen, die an Personen in Ihrer Organisation gesendet werden**.</span><span class="sxs-lookup"><span data-stu-id="62f17-105">You can **only recall messages that are sent to people in your organization**.</span></span> <span data-ttu-id="62f17-106">Wenn die Nachricht beispielsweise an eine gmail-Adresse gesendet wurde, können Sie Sie nicht mehr abrufen.</span><span class="sxs-lookup"><span data-stu-id="62f17-106">If the message was sent to a Gmail address, for example, you can't recall it.</span></span>
- <span data-ttu-id="62f17-107">Sie können **nur Nachrichten abrufen, die von Outlook 2016 auf dem PC gesendet wurden**.</span><span class="sxs-lookup"><span data-stu-id="62f17-107">You can **only recall messages sent from Outlook 2016 on the PC**.</span></span> <span data-ttu-id="62f17-108">Wenn ein Benutzer eine Nachricht mit Outlook für Mac oder Outlook im Internet sendet, kann er nicht mehr daran erinnert werden.</span><span class="sxs-lookup"><span data-stu-id="62f17-108">If a user sends a message using Outlook for Mac or Outlook on the web, you can't recall it.</span></span>

<span data-ttu-id="62f17-109">So rufen Sie eine e-Mail-Nachricht auf oder ersetzen Sie:</span><span class="sxs-lookup"><span data-stu-id="62f17-109">To recall or replace an email message:</span></span>

1. <span data-ttu-id="62f17-110">Wählen Sie im Ordnerbereich auf der linken Seite des Outlook-Fensters den Ordner "Gesendete Elemente" aus.</span><span class="sxs-lookup"><span data-stu-id="62f17-110">In the folder pane on the left of the Outlook window, select the Sent Items folder.</span></span>
1. <span data-ttu-id="62f17-111">Doppelklicken Sie auf die Nachricht, die Sie abrufen möchten, um Sie zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="62f17-111">Double-click the message you want to recall to open it.</span></span>
1. <span data-ttu-id="62f17-112">Wählen Sie die Registerkarte **Nachricht** aus, und wählen Sie dann **Aktionen**  >  **Rückruf dieser Nachricht**aus.</span><span class="sxs-lookup"><span data-stu-id="62f17-112">Select the **Message** tab, and then select **Actions** > **Recall This Message**.</span></span>
1. <span data-ttu-id="62f17-113">Wählen Sie **Ungelesene Kopien dieser Nachricht löschen** oder **Ungelesene Kopien löschen aus, und ersetzen Sie Sie durch eine neue Nachricht**, und wählen Sie dann **OK**aus.</span><span class="sxs-lookup"><span data-stu-id="62f17-113">Select **Delete unread copies of this message** or **Delete unread copies and replace with a new message**, and then select **OK**.</span></span>
1. <span data-ttu-id="62f17-114">Wenn Sie eine Ersatznachricht senden, verfassen Sie die Nachricht, und wählen Sie dann **senden**aus.</span><span class="sxs-lookup"><span data-stu-id="62f17-114">If you're sending a replacement message, compose the message, and then select **Send**.</span></span>
1. <span data-ttu-id="62f17-115">Der Erfolg oder Misserfolg eines Nachrichtenrückrufs hängt von den Einstellungen des Empfängers in Outlook ab.</span><span class="sxs-lookup"><span data-stu-id="62f17-115">The success or failure of a message recall depends on the recipient's settings in Outlook.</span></span> <span data-ttu-id="62f17-116">Schritte zum Überprüfen des Rückrufs finden Sie in [diesem Artikel](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span><span class="sxs-lookup"><span data-stu-id="62f17-116">For steps to check on the recall, see [this article](https://support.office.com/article/35027f88-d655-4554-b4f8-6c0729a723a0).</span></span>

<span data-ttu-id="62f17-117">Suchen nach und Löschen von E-Mail-Nachrichten in der Organisation</span><span class="sxs-lookup"><span data-stu-id="62f17-117">Search for and delete email messages in your organization</span></span>

- <span data-ttu-id="62f17-118">Wenn Sie kein globaler Administrator sind, muss Ihr Konto zur eDiscovery-Manager-Rolle oder zur Verwaltungsrolle "Compliance Search" hinzugefügt werden, um nach Nachrichten zu suchen.</span><span class="sxs-lookup"><span data-stu-id="62f17-118">If you're not a global admin, your account must be added to the eDiscovery Manager role or Compliance Search management role to search for messages.</span></span> <span data-ttu-id="62f17-119">Wenn Sie Nachrichten löschen möchten, müssen Sie der Rollengruppe "Organisationsverwaltung" oder der Rolle "Such-und Lösch Verwaltung" beitreten.</span><span class="sxs-lookup"><span data-stu-id="62f17-119">To delete messages, you'll need to join the Organization Management role group or the Search and Purge management role.</span></span> <span data-ttu-id="62f17-120">Berechtigungen für diese Rollen werden im [Security and Compliance Center](https://go.microsoft.com/fwlink/?linkid=2083731)zugewiesen.</span><span class="sxs-lookup"><span data-stu-id="62f17-120">Permissions for these roles are assigned in the [Security and compliance center](https://go.microsoft.com/fwlink/?linkid=2083731).</span></span>
- <span data-ttu-id="62f17-121">[Erstellen Sie eine Inhaltssuche](https://docs.microsoft.com/microsoft-365/compliance/content-search) , um die zu löschende Nachricht zu suchen.</span><span class="sxs-lookup"><span data-stu-id="62f17-121">[Create a content search](https://docs.microsoft.com/microsoft-365/compliance/content-search) to find the message to delete.</span></span>
- <span data-ttu-id="62f17-122">Stellen [Sie eine Verbindung mit Security and Compliance Center PowerShell her](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="62f17-122">[Connect to Security and Compliance Center PowerShell](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/connect-to-scc-powershell?view=exchange-ps).</span></span>

<span data-ttu-id="62f17-123">Wenn Sie die mehrstufige Authentifizierung verwenden, lesen Sie die Informationen unter [Connect to Microsoft 365 Security and Compliance Center PowerShell using Multi-Factor Authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="62f17-123">If you're using multi-factor authentication, see [Connect to Microsoft 365 security and Compliance Center PowerShell using multi-factor authentication](https://docs.microsoft.com/powershell/exchange/office-365-scc/connect-to-scc-powershell/mfa-connect-to-scc-powershell?view=exchange-ps).</span></span>