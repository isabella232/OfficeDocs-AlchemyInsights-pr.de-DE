---
title: Beispiel für Microsoft Defender für Office 365-Antiphishingrichtlinie
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552422"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a><span data-ttu-id="d14a7-102">Beispiel für Microsoft Defender für Office 365-Antiphishingrichtlinie</span><span class="sxs-lookup"><span data-stu-id="d14a7-102">Example Microsoft Defender for Office 365 anti-phishing policy</span></span>

<span data-ttu-id="d14a7-103">Mit diesen Einstellungen wird eine Richtlinie namens *"Domäne und CEO" aktiviert.*</span><span class="sxs-lookup"><span data-stu-id="d14a7-103">These settings enable a policy called *Domain and CEO*.</span></span> <span data-ttu-id="d14a7-104">Diese Richtlinie bietet Sowohl Benutzer- als auch Domänenschutz vor Identitätswechseln und wendet die Richtlinie dann auf alle E-Mails an, die von Benutzern innerhalb der Domäne empfangen werden.</span><span class="sxs-lookup"><span data-stu-id="d14a7-104">This policy provides both user and domain protection from impersonation and then applies the policy to all email received by users within the domain.</span></span> <span data-ttu-id="d14a7-105">Fügen Sie zunächst die folgenden Informationen hinzu, um die Richtlinie zu erstellen:</span><span class="sxs-lookup"><span data-stu-id="d14a7-105">First, add the following information to create the policy:</span></span>

- <span data-ttu-id="d14a7-106">**Name**: Domänen- und **CEO-Beschreibung**: Stellt sicher, dass der CEO und Ihre Domäne nicht als identitätswechselt werden.</span><span class="sxs-lookup"><span data-stu-id="d14a7-106">**Name**: Domain and CEO **Description**: Ensures that the CEO and your domain are not being impersonated.</span></span>
  <span data-ttu-id="d14a7-107">**Angewendet auf**: Select **Die Empfängerdomäne ist**.</span><span class="sxs-lookup"><span data-stu-id="d14a7-107">**Applied to**: Select **The recipient domain is**.</span></span> <span data-ttu-id="d14a7-108">Wählen **Sie unter Alle diese** Die Option **Auswählen** aus, und wählen Sie dann eine Domäne aus.</span><span class="sxs-lookup"><span data-stu-id="d14a7-108">Under **Any of these**, select **Choose**, and then select a domain.</span></span> <span data-ttu-id="d14a7-109">Wählen Sie **+ Hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="d14a7-109">Select **+ Add**.</span></span> <span data-ttu-id="d14a7-110">Aktivieren Sie das Kontrollkästchen neben dem Namen der Domäne in der Liste (z. B. contoso.com *),* und wählen Sie dann **Hinzufügen aus.**</span><span class="sxs-lookup"><span data-stu-id="d14a7-110">Select the check box next to the name of the domain in the list (for example, *contoso.com*), and then select **Add**.</span></span> <span data-ttu-id="d14a7-111">Wählen Sie **Fertig** aus.</span><span class="sxs-lookup"><span data-stu-id="d14a7-111">Select **Done**.</span></span>
- <span data-ttu-id="d14a7-112">Nachdem die Richtlinie erstellt wurde, können Sie die Richtlinie mithilfe der folgenden Optionen optimieren:</span><span class="sxs-lookup"><span data-stu-id="d14a7-112">After the policy is created, you can fine-tune the policy by using the following options:</span></span>
  - <span data-ttu-id="d14a7-113">**Hinzufügen von Benutzern zum Schützen:** Fügen Sie in diesem Beispiel mindestens die E-Mail-Adresse des CEO hinzu.</span><span class="sxs-lookup"><span data-stu-id="d14a7-113">**Add users to protect:** For this example, add the CEO's email address, at a minimum.</span></span>
  - <span data-ttu-id="d14a7-114">**Zu schützende** Domänen hinzufügen: Fügen Sie die Organisationsdomäne hinzu, die das Büro des CEO enthält.</span><span class="sxs-lookup"><span data-stu-id="d14a7-114">**Add domains to protect**: Add the organizational domain that includes the office of the CEO.</span></span>
  - <span data-ttu-id="d14a7-115">**Aktionen auswählen:** Wenn E-Mails von einem identitätswechselten Benutzer gesendet **werden,** wählen Sie **Nachricht** an eine andere E-Mail-Adresse umleiten aus, und geben Sie dann die E-Mail-Adresse des Sicherheitsadministrators ein (z. B. *securityadmin@contoso.com*).</span><span class="sxs-lookup"><span data-stu-id="d14a7-115">**Choose actions**: For **If email is sent by an impersonated user**, select **Redirect message to another email address**, and then enter the email address of the security administrator (for example, *securityadmin@contoso.com*).</span></span> <span data-ttu-id="d14a7-116">For **If email is sent by an impersonated domain,** select Quarantine the **message**.</span><span class="sxs-lookup"><span data-stu-id="d14a7-116">For **If email is sent by an impersonated domain**, select **Quarantine the message**.</span></span>
  - <span data-ttu-id="d14a7-117">**Postfachintelligenz:** Diese Option ist standardmäßig ausgewählt, wenn Sie eine neue Antiphishingrichtlinie erstellen.</span><span class="sxs-lookup"><span data-stu-id="d14a7-117">**Mailbox intelligence**: By default, this option is selected when you create a new anti-phishing policy.</span></span> <span data-ttu-id="d14a7-118">Lassen Sie diese Einstellung auf **Ein**, um optimale Ergebnisse zu erzielen.</span><span class="sxs-lookup"><span data-stu-id="d14a7-118">Leave this setting **On** for best results.</span></span>
  - <span data-ttu-id="d14a7-119">**Hinzufügen vertrauenswürdiger Absender und Domänen:** Definieren Sie in diesem Beispiel keine Außerkraftsetzungen.</span><span class="sxs-lookup"><span data-stu-id="d14a7-119">**Add trusted senders and domains:** For this example, don't define any overrides.</span></span>
- <span data-ttu-id="d14a7-120">Nachdem Sie Ihre Einstellungen überprüft haben, wählen Sie Diese Richtlinie **erstellen** oder **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="d14a7-120">Once you've reviewed your settings, select **Create this policy** or **Save**, as appropriate.</span></span>

<span data-ttu-id="d14a7-121">Weitere Informationen finden Sie unter [Antiphishingrichtlinien in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span><span class="sxs-lookup"><span data-stu-id="d14a7-121">To learn more, see [Anti-phishing policies in Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).</span></span>
