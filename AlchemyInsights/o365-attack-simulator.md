---
title: 2681-Angriffs Simulator in Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305331"
---
# <a name="attack-simulator-in-office-365"></a><span data-ttu-id="121c1-102">Angriffssimulator in Office 365</span><span class="sxs-lookup"><span data-stu-id="121c1-102">Attack Simulator in Office 365</span></span>

- <span data-ttu-id="121c1-103">Fehlt Ihnen der Angriffs Simulator?</span><span class="sxs-lookup"><span data-stu-id="121c1-103">Are you missing Attack Simulator?</span></span> <span data-ttu-id="121c1-104">Angriffs Simulator erfordert **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** oder **Office 365 Enterprise E5**.</span><span class="sxs-lookup"><span data-stu-id="121c1-104">Attack Simulator requires **Office 365 Advanced Threat Protection Plan 2 (ATP Plan 2)** or **Office 365 Enterprise E5**.</span></span> <span data-ttu-id="121c1-105">Der Angriffs Simulator ist **nicht** in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3 oder any Office 365 Business Subscriptions enthalten.</span><span class="sxs-lookup"><span data-stu-id="121c1-105">Attack Simulator is **not** included in Office 365 Advanced Threat Protection Plan 1 (ATP Plan 1), Office 365 Enterprise E3, or any Office 365 Business subscriptions.</span></span>

- <span data-ttu-id="121c1-106">Das Konto, das Sie zum Starten simulierter Angriffe verwenden, erfordert globale Administrator-oder Sicherheitsadministratorberechtigungen und mehrstufige Authentifizierung (MFA).</span><span class="sxs-lookup"><span data-stu-id="121c1-106">The account you use to launch simulated attacks requires global administrator or security administrator permissions and multi-factor authentication (MFA).</span></span> <span data-ttu-id="121c1-107">Weitere Informationen zu Anforderungen für den Angriffs Simulator finden Sie in [diesem Thema](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="121c1-107">For more information about Attack Simulator requirements, see [this topic](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).</span></span>

- <span data-ttu-id="121c1-108">Wichtige Dinge, die Sie über **Brute-Force-Kenn Wort** Angriffssimulationen wissen sollten:</span><span class="sxs-lookup"><span data-stu-id="121c1-108">Important things to know about **Brute Force Password** attack simulations:</span></span>

  - <span data-ttu-id="121c1-109">Wenn für das Zielkonto ein MFA aktiviert ist und das Kennwort richtig erraten wurde, wird das Konto nicht als kompromittiert angezeigt (der zweite Authentifizierungs Faktor ist unvollständig).</span><span class="sxs-lookup"><span data-stu-id="121c1-109">If the target account has MFA enabled and the password was guessed correctly, the account will not show as compromised (the second authentication factor will be incomplete).</span></span>

  - <span data-ttu-id="121c1-110">Die Kennwortdatei darf nicht größer als 10 MB sein.</span><span class="sxs-lookup"><span data-stu-id="121c1-110">The password file can't be larger than 10 MB.</span></span> <span data-ttu-id="121c1-111">Verwenden Sie ein Kennwort pro Zeilen, und fügen Sie eine leere Zeilen (Wagenrücklauf) nach dem letzten Kennwort in der Liste ein.</span><span class="sxs-lookup"><span data-stu-id="121c1-111">Use one password per line, and include a blank line (carriage return) after the last password in the list.</span></span>

- <span data-ttu-id="121c1-112">Wichtige Dinge, die Sie über **Speer-Phishing** -Anfügungs Simulationen wissen sollten:</span><span class="sxs-lookup"><span data-stu-id="121c1-112">Important things to know about **Spear Phishing** attach simulations:</span></span>

  - <span data-ttu-id="121c1-113">Durch Entwurf können Sie keinen benutzerdefinierten Wert für die **URL des Phishing-Anmeldeservers**angeben.</span><span class="sxs-lookup"><span data-stu-id="121c1-113">By design, you can't provide a custom value for **Phishing login server URL**.</span></span>

  - <span data-ttu-id="121c1-114">Wenn ein Empfänger das [Add-in "Berichtsnachricht aktivieren](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) " verwendet, um die Nachricht als Phishing zu melden, erhalten Sie möglicherweise keine Benachrichtigungen für die Nachricht (da es sich um einen simulierten Angriff handelt).</span><span class="sxs-lookup"><span data-stu-id="121c1-114">If a recipient uses the [Enable the Report Message add-in](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) to report the message as phishing, you might not receive alerts for the message (because this is a simulated attack).</span></span>

- <span data-ttu-id="121c1-115">Berichte: Wenn der simulierte Angriff abgeschlossen ist, können Sie auf **Angriffs Details** klicken, um den Bericht anzuzeigen.</span><span class="sxs-lookup"><span data-stu-id="121c1-115">Reports: After the simulated attack is complete, you can click **Attack Details** to see the report.</span></span>

- <span data-ttu-id="121c1-116">Ausführliche Anweisungen und neue Features in Attack Simulator finden Sie unter [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span><span class="sxs-lookup"><span data-stu-id="121c1-116">For detailed instructions and new features in Attack Simulator, see [Attack Simulator in Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).</span></span>
