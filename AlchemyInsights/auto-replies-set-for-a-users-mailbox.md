---
title: Festlegen von automatischen Antworten für ein Postfach
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000761"
- "3514"
ms.openlocfilehash: 03c530e7ce5f00fce2222cf9993930b97e5a2818
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715128"
---
# <a name="set-auto-replies-for-a-users-mailbox"></a><span data-ttu-id="fe94f-102">Festlegen von automatischen Antworten für das Postfach eines Benutzers</span><span class="sxs-lookup"><span data-stu-id="fe94f-102">Set auto replies for a user's mailbox</span></span>

<span data-ttu-id="fe94f-103">**Methode 1**</span><span class="sxs-lookup"><span data-stu-id="fe94f-103">**Method 1**</span></span>

1. <span data-ttu-id="fe94f-104">Melden Sie sich im Microsoft 365-Portal an.</span><span class="sxs-lookup"><span data-stu-id="fe94f-104">Sign in to the Microsoft 365 portal.</span></span>

2. <span data-ttu-id="fe94f-105">Wechseln Sie zu **Benutzer > Aktive Benutzer** (oder **Gruppen > Freigegebene Postfächer**, wenn Sie diese Option für ein freigegebenes Postfach festlegen).</span><span class="sxs-lookup"><span data-stu-id="fe94f-105">Go to **Users > Active users** (or **Groups > Shared mailboxes** if you set this on a shared mailbox).</span></span>

3. <span data-ttu-id="fe94f-106">Wählen Sie einen Benutzer aus, der über ein Microsoft Exchange-Postfach verfügt.</span><span class="sxs-lookup"><span data-stu-id="fe94f-106">Select a user who has a Microsoft Exchange mailbox.</span></span>

4. <span data-ttu-id="fe94f-107">Wechseln Sie im Kontextmenü rechts zu **E-Mail-Einstellungen > Automatische Antworten** (sofern es sich um ein freigegebenes Postfach handelt, klicken Sie einfach auf **Automatische Antworten** im Kontextmenü).</span><span class="sxs-lookup"><span data-stu-id="fe94f-107">On the fly-out menu on the right, go to **Mail settings > Automatic replies** (if it's a shared mailbox, just click **Automatic replies** on the fly-out).</span></span>

<span data-ttu-id="fe94f-108">**Methode 2**</span><span class="sxs-lookup"><span data-stu-id="fe94f-108">**Method 2**</span></span>

1. <span data-ttu-id="fe94f-109">Melden Sie sich mit Ihren Anmeldeinformationen als Administrator beim Microsoft 365-Verwaltungsportal an.</span><span class="sxs-lookup"><span data-stu-id="fe94f-109">Sign in to the Microsoft 365 admin portal by using administrator credentials.</span></span>

2. <span data-ttu-id="fe94f-110">Erweitern Sie **Admin Center**, und klicken Sie auf **Exchange**.</span><span class="sxs-lookup"><span data-stu-id="fe94f-110">Expand **Admin Centers**, and then click **Exchange**.</span></span>

3. <span data-ttu-id="fe94f-111">Klicken Sie in der oberen rechten Ecke auf das Bild, klicken Sie auf **Ein anderer Benutzer**, und wählen Sie dann das Benutzerpostfach aus, das Sie ändern möchten.</span><span class="sxs-lookup"><span data-stu-id="fe94f-111">Click the picture in the upper-right corner, click **Another User**, and then select the user mailbox that you want to change.</span></span>

4. <span data-ttu-id="fe94f-112">Wählen Sie auf der linken Seite **Optionen** aus, klicken Sie auf **E-Mail organisieren**, und klicken Sie dann auf **Automatische Antworten.**</span><span class="sxs-lookup"><span data-stu-id="fe94f-112">On the left side, select **Options**, click **Organize E-mail**, and then click **Automatic replies.**</span></span>

<span data-ttu-id="fe94f-113">**Methode 3**</span><span class="sxs-lookup"><span data-stu-id="fe94f-113">**Method 3**</span></span>

<span data-ttu-id="fe94f-114">Führen Sie das folgenden Cmdlet in Exchange Online PowerShell aus:</span><span class="sxs-lookup"><span data-stu-id="fe94f-114">Run the following cmdlet in Exchange Online PowerShell:</span></span>

<span data-ttu-id="fe94f-115">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="fe94f-115">PowerShellCopy</span></span>

```
    Set-MailboxAutoReplyConfiguration
```

<span data-ttu-id="fe94f-116">Weitere Informationen zu diesem Cmdlet finden Sie unter [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span><span class="sxs-lookup"><span data-stu-id="fe94f-116">For more information about this cmdlet, see [Set-MailboxAutoReplyConfiguration](https://docs.microsoft.com/powershell/module/exchange/mailboxes/set-mailboxautoreplyconfiguration).</span></span>
