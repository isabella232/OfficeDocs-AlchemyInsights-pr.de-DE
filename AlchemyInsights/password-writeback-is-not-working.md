---
title: Kennwortrückschreiben funktioniert nicht
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232720"
---
# <a name="password-writeback-is-not-working"></a><span data-ttu-id="b8aa0-102">Kennwortrückschreiben funktioniert nicht</span><span class="sxs-lookup"><span data-stu-id="b8aa0-102">Password Writeback is not working</span></span>

<span data-ttu-id="b8aa0-103">**Ich habe Probleme beim Konfigurieren des Kennwortrückschreibens**</span><span class="sxs-lookup"><span data-stu-id="b8aa0-103">**I'm having problems configuring password writeback**</span></span>

- <span data-ttu-id="b8aa0-104">Kennwortrückschreiben ist ein Premium-Feature.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-104">Password writeback is a premium feature.</span></span>
- <span data-ttu-id="b8aa0-105">Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen kennen:</span><span class="sxs-lookup"><span data-stu-id="b8aa0-105">Make sure that you understand the licensing requirements:</span></span>
  - <span data-ttu-id="b8aa0-106">Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-106">You must have at least one license assigned in your organization</span></span>
  - <span data-ttu-id="b8aa0-107">**Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365)-SKU oder Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="b8aa0-107">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
  - <span data-ttu-id="b8aa0-108">**Cloud- und/oder** lokale Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-108">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="b8aa0-109">Weitere Informationen zu Den Lizenzierungsanforderungen finden Sie unter Lizenzierungsanforderungen für die [Self-Service-Kennwortzurücksetzung in Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-109">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span></span>
- <span data-ttu-id="b8aa0-110">Sie verfügen über mindestens ein Administratorkonto und ein Testbenutzerkonto mit einer der entsprechenden Lizenz.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-110">You have at least one administrator account and one test user account with one of the appropriate license.</span></span>
- <span data-ttu-id="b8aa0-111">Sie müssen Azure AD Connect mit dem primären Domänencontrolleremulator verbinden, damit das Kennwortrückschreiben funktioniert.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-111">You must connect Azure AD Connect to the Primary Domain Controller Emulator for password writeback to work.</span></span> <span data-ttu-id="b8aa0-112">Sie können Azure AD Connect für die Verwendung eines  primären Domänencontrollers konfigurieren, indem Sie mit der rechten Maustaste auf die Eigenschaften des Active Directory-Synchronisierungsconnector klicken und dann **Verzeichnispartitionen konfigurieren.**</span><span class="sxs-lookup"><span data-stu-id="b8aa0-112">You can configure Azure AD Connect to use a Primary Domain Controller by right clicking on the **properties** of the Active Directory synchronization connector, then selecting **configure directory partitions**.</span></span> <span data-ttu-id="b8aa0-113">Suchen Sie von dort aus nach **dem** Abschnitt mit den Einstellungen für die Domänencontrollerverbindung, und aktivieren Sie das Kontrollkästchen mit der Bezeichnung **"Nur bevorzugte Domänencontroller verwenden".**</span><span class="sxs-lookup"><span data-stu-id="b8aa0-113">From there, look for the **domain controller connection settings** section and check the box titled **only use preferred domain controllers**.</span></span>
  > [!NOTE]
  > <span data-ttu-id="b8aa0-114">Wenn es sich bei dem bevorzugten DC nicht um einen PDC-Emulator handelt, kontaktiert Azure AD Connect weiterhin das PDC für das Kennwortrückschreiben.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-114">If the preferred DC is not a PDC emulator, Azure AD Connect will still reach out to the PDC for password writeback.</span></span>
- <span data-ttu-id="b8aa0-115">Die Kennwortzurücksetzung wurde in Ihrem Mandanten konfiguriert und aktiviert.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-115">Password reset has been configured and enabled in your tenant.</span></span> <span data-ttu-id="b8aa0-116">Weitere Informationen finden Sie unter "Aktivieren der Benutzer [zum Zurücksetzen ihrer Azure AD-Kennwörter".](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-116">For more information, see [Enable users to reset their Azure AD passwords](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started).</span></span>
- <span data-ttu-id="b8aa0-117">Stellen Sie sicher, dass das Administratorkonto, das zum Aktivieren des Kennwortrückschreibens verwendet wird, ein Cloudadministratorkonto ist (erstellt in Azure AD und nicht in der lokalen AD-Bereitstellung)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-117">Make sure that the administrator account being used to enable Password Writeback is a cloud administrator account (created in Azure AD not on-premises AD)</span></span>
- <span data-ttu-id="b8aa0-118">Sie verfügen über eine lokale Ad-Bereitstellung mit einer oder mehreren Gesamtstrukturen, in der Windows Server 2008 R2, Windows Server 2012 oder Windows Server 2012 R2 ausgeführt wird, in der die neuesten Service Packs installiert sind.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-118">You have a single or multi-forest AD on-premises deployment running Windows Server 2008 R2, Windows Server 2012, or Windows Server 2012 R2 with the latest service packs installed</span></span>
- <span data-ttu-id="b8aa0-119">Sie haben das Azure AD Connect-Tool installiert und Ihre AD-Umgebung für die Synchronisierung mit der Cloud vorbereitet.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-119">You have the Azure AD Connect tool installed and you have prepared your AD environment for synchronization to the cloud.</span></span> <span data-ttu-id="b8aa0-120">Stellen Sie vor dem Testen des Kennwortrückschreibens sicher, dass Sie zuerst einen vollständigen Import und eine vollständige Synchronisierung aus AD und Azure AD in Azure AD Connect abschließen.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-120">Before testing password writeback, make sure that you first complete a full import and full sync from both AD and Azure AD in Azure AD Connect.</span></span>
- <span data-ttu-id="b8aa0-121">Weitere Informationen finden Sie unter einer vollständigen Synchronisierung [und einem vollständigen Import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-121">To learn more, see how to do a [full sync and full import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)</span></span>

<span data-ttu-id="b8aa0-122">**I'm having a problem with password writeback connectivity**</span><span class="sxs-lookup"><span data-stu-id="b8aa0-122">**I'm having a problem with password writeback connectivity**</span></span>

1. <span data-ttu-id="b8aa0-123">Herunterladen und Aktivieren der neuesten Version von [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-123">Download and enable the latest version of [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)</span></span>
2. <span data-ttu-id="b8aa0-124">Firewallkonfiguration: Das Azure AD -Connect-Tool (1.1.443 und höher) benötigt **ausgehenden HTTPS-Zugriff** auf:</span><span class="sxs-lookup"><span data-stu-id="b8aa0-124">Firewall configuration: The Azure AD Connect tool (1.1.443 and above) will need **outbound HTTPS** access to:</span></span>
    - <span data-ttu-id="b8aa0-125">passwordreset.microsoftonline.com</span><span class="sxs-lookup"><span data-stu-id="b8aa0-125">passwordreset.microsoftonline.com</span></span>
    - <span data-ttu-id="b8aa0-126">servicebus.windows.networks</span><span class="sxs-lookup"><span data-stu-id="b8aa0-126">servicebus.windows.networks</span></span>
3. <span data-ttu-id="b8aa0-127">Zulassen, dass Leerlaufverbindungen mindestens 2-3 Minuten lang bestehen bleiben</span><span class="sxs-lookup"><span data-stu-id="b8aa0-127">Allow idle connections to persist for at least 2-3 minutes</span></span>

<span data-ttu-id="b8aa0-128">**Ich habe weiterhin Probleme mit dem Kennwortrückschreiben**</span><span class="sxs-lookup"><span data-stu-id="b8aa0-128">**I'm still having problems with password writeback**</span></span>

- <span data-ttu-id="b8aa0-129">Wenn sie weiterhin Probleme haben, versuchen Sie, den Kennwortrückschreibendienst im Azure AD -Connect-Tool zu deaktivieren und erneut zu aktivieren.</span><span class="sxs-lookup"><span data-stu-id="b8aa0-129">If you are still having difficulty, try disabling and re-enabling the password writeback service in the Azure AD Connect tool</span></span>
- <span data-ttu-id="b8aa0-130">Weitere Informationen finden Sie unter Deaktivieren und erneutes Aktivieren [des Kennwortrückschreibens.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span><span class="sxs-lookup"><span data-stu-id="b8aa0-130">To learn more, see how to [disable and re-enable password writeback](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)</span></span>
