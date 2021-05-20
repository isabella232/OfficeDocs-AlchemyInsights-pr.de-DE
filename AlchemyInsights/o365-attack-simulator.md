---
title: 2681 Attack Simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: e7d71fdb77b4a047c1998e9aba75cdd469a936a8
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52545725"
---
# <a name="attack-simulator-in-microsoft-365"></a><span data-ttu-id="0eda8-102">Angriffssimulator in Microsoft 365</span><span class="sxs-lookup"><span data-stu-id="0eda8-102">Attack Simulator in Microsoft 365</span></span>

- <span data-ttu-id="0eda8-103">Fehlt Ihnen der Angriffssimulator?</span><span class="sxs-lookup"><span data-stu-id="0eda8-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="0eda8-104">Der Angriffssimulator erfordert **Microsoft Defender für Office 365 Plan 2** oder Office 365 Enterprise **E5**.</span><span class="sxs-lookup"><span data-stu-id="0eda8-104">Attack Simulator requires **Microsoft Defender for Office 365 Plan 2** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="0eda8-105">Der **Angriffssimulator ist** nicht in Microsoft Defender für Office 365 Plan 1, Office 365 Enterprise E3 oder in Microsoft 365 Apps for Business enthalten.</span><span class="sxs-lookup"><span data-stu-id="0eda8-105">Attack Simulator is **not** included in Microsoft Defender for Office 365 Plan 1, Office 365 Enterprise E3, or any Microsoft 365 Apps for business subscriptions.</span></span>

- <span data-ttu-id="0eda8-106">Für das Konto, das Sie zum Starten simulierter Angriffe verwenden, sind globale Administrator- oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (MFA) erforderlich.</span><span class="sxs-lookup"><span data-stu-id="0eda8-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="0eda8-107">Weitere Informationen zu den Anforderungen des Angriffssimulators finden Sie [in diesem Thema.](/microsoft-365/security/office-365-security/attack-simulator)</span><span class="sxs-lookup"><span data-stu-id="0eda8-107">For more information about Attack Simulator requirements, see [this topic](/microsoft-365/security/office-365-security/attack-simulator).</span></span>

- <span data-ttu-id="0eda8-108">Wichtige Informationen zu **Brute Force Password-Angriffssimulationen:**</span><span class="sxs-lookup"><span data-stu-id="0eda8-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="0eda8-109">Wenn das Zielkonto MFA aktiviert hat und das Kennwort richtig erraten wurde, wird das Konto nicht als gefährdet angezeigt (der zweite Authentifizierungsfaktor ist unvollständig).</span><span class="sxs-lookup"><span data-stu-id="0eda8-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="0eda8-110">Die Kennwortdatei darf nicht größer als 10 MB sein.</span><span class="sxs-lookup"><span data-stu-id="0eda8-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="0eda8-111">Verwenden Sie ein Kennwort pro Zeile, und fügen Sie eine leere Zeile (Wagenrücklauf) nach dem letzten Kennwort in die Liste ein.</span><span class="sxs-lookup"><span data-stu-id="0eda8-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="0eda8-112">Wichtige Informationen zu **Spear Phishing-Anfügen-Simulationen:**</span><span class="sxs-lookup"><span data-stu-id="0eda8-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="0eda8-113">Standardmäßig können Sie keinen benutzerdefinierten Wert für die **Phishing-Anmeldeserver-URL angeben.**</span><span class="sxs-lookup"><span data-stu-id="0eda8-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="0eda8-114">Wenn ein Empfänger das [Add-In](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) Nachricht melden aktivieren verwendet, um die Nachricht als Phishing zu melden, erhalten Sie möglicherweise keine Benachrichtigungen für die Nachricht (da es sich um einen simulierten Angriff handelt).</span><span class="sxs-lookup"><span data-stu-id="0eda8-114">If a recipient uses the [Enable the Report Message add-in](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="0eda8-115">Berichte: Nach Abschluss des simulierten Angriffs können Sie auf **Angriffsdetails klicken,** um den Bericht anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="0eda8-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="0eda8-116">Ausführliche Anweisungen und neue Features in Attack Simulator finden Sie unter [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="0eda8-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).</span></span>
