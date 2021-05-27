---
title: Regeln zur Verringerung der Angriffsfläche
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/25/2021
ms.locfileid: "52651486"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="e5cf3-102">Regeln zur Verringerung der Angriffsfläche</span><span class="sxs-lookup"><span data-stu-id="e5cf3-102">Attack surface reduction rules</span></span>

<span data-ttu-id="e5cf3-103">Das Ausschließen von Dateien oder Ordnern kann den Schutz durch Regeln zur Verringerung der Angriffsfläche erheblich beeinträchtigen.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="e5cf3-104">Dateien, die durch eine Regel blockiert worden wären, dürfen ausgeführt werden, und es wird kein Bericht oder Ereignis aufgezeichnet.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="e5cf3-105">Ein Ausschluss gilt für alle Regeln, die Ausschlüsse zulassen.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="e5cf3-106">ASR-Ausschlüsse verwenden dieselbe Syntax wie Microsoft Defender Antivirus-Ausschlüsse.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="e5cf3-107">Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen für Microsoft Defender Antivirus-Scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="e5cf3-108">Um Probleme zu vermeiden, lesen Sie [Häufige Fehler, die beim Festlegen von Ausschlüssen vermieden werden sollten](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="e5cf3-109">Nicht alle ASR-Regeln unterstützen Ausschlüsse.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="e5cf3-110">Informationen zur Überprüfung, ob Ihre Regel Ausschlüsse unterstützt, finden Sie in der Tabelle [Regeln zur Verringerung der Angriffsfläche](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="e5cf3-111">Regeln zur Verringerung der Angriffsfläche</span><span class="sxs-lookup"><span data-stu-id="e5cf3-111">Attack surface reduction rules</span></span>

<span data-ttu-id="e5cf3-112">Die Angriffsfläche Ihrer Organisation enthält alle Stellen, an denen ein Angreifer Geräte oder Netzwerke der Organisation gefährden könnte.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="e5cf3-113">Die Verringerung ihrer Angriffsoberfläche bedeutet, die Geräte und das Netzwerk des Unternehmens zu schützen, sodass Angreifer weniger Möglichkeiten haben, Angriffe auszuführen.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="e5cf3-114">Das Konfigurieren von Regeln zur Verringerung der Angriffsfläche in Microsoft Defender für Endpunkt kann dabei hilfreich sein.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="e5cf3-115">Weitere Informationen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="e5cf3-115">For more information, see:</span></span>

- [<span data-ttu-id="e5cf3-116">Zuordnen des ASR-Regel-GUID zu Namen</span><span class="sxs-lookup"><span data-stu-id="e5cf3-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="e5cf3-117">Voraussetzungen der ASR-Regeln:</span><span class="sxs-lookup"><span data-stu-id="e5cf3-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="e5cf3-118">Windows 10, Version 1709 oder höher</span><span class="sxs-lookup"><span data-stu-id="e5cf3-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="e5cf3-119">Windows 10 Enterprise, Version 1709 oder höher</span><span class="sxs-lookup"><span data-stu-id="e5cf3-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="e5cf3-120">Windows Server, Version 1803 (halbjährlicher Kanal) oder höher</span><span class="sxs-lookup"><span data-stu-id="e5cf3-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="e5cf3-121">Identifizieren Sie den richtigen, anzuwendenden Ausschluss.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="e5cf3-122">Suchen Sie im Microsoft-Windows-Windows Defender/ Betriebsprotokoll nach eventID 1121 oder 1122.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="e5cf3-123">Werten Sie das Blockierungsszenario und den Kontext aus und bestätigen Sie, dass dieses Szenario entsperrt werden soll.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="e5cf3-124">Lesen Sie den Pfadwert in den Ereignisdetails. Dies ist der Wert, der den Ausschluss definiert.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="e5cf3-125">Machen Sie den Ausschluss so streng wie möglich.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="e5cf3-126">Wenden Sie bei Bedarf einen Platzhalter an (ersetzen Sie beispielsweise die Benutzervariable).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="e5cf3-127">Wenden Sie den Ausschluss entsprechend Ihren Bereitstellungsanforderungen an.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="e5cf3-128">Weitere Informationen finden Sie unter [Anpassen der Regeln zur Verringerung der Angriffsfläche](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="e5cf3-129">Ausschluss wird nicht anerkannt</span><span class="sxs-lookup"><span data-stu-id="e5cf3-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="e5cf3-130">Bestimmen Sie, ob die Regel Ausschlüsse unterstützt.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="e5cf3-131">Weitere Informationen finden Sie unter [Anpassen der Regeln zur Verringerung der Angriffsfläche](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="e5cf3-132">Überprüfen Sie die angewendeten Ausschlüsse und überprüfen Sie anhand der Ereignisdaten, ob Tippfehler oder falsch interpretierte Platzhalter vorhanden sind.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="e5cf3-133">Weitere Informationen finden Sie unter [Unterstützte Ausschlusstypen](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="e5cf3-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="e5cf3-134">Wenn die Auswirkung der Regel zu hoch ist, sollten Sie die Regel (zurück) in den Überwachungsmodus verschieben, um eine weitere Validierung durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="e5cf3-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="e5cf3-135">Weitere Informationen finden Sie unter [Testen der Funktionalität der Features von Microsoft Defender für Endpunkte im Überwachungsmodus](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="e5cf3-136">Sammeln Sie Supportdaten, um einen Supportfall mit diesem Befehl zu öffnen:</span><span class="sxs-lookup"><span data-stu-id="e5cf3-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="e5cf3-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="e5cf3-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="e5cf3-138">Weitere Informationen finden Sie unter [Probleme mit Onboarding-Computern in Microsoft Defender für Endpunkte](issues-with-onboarding-machines.md).</span><span class="sxs-lookup"><span data-stu-id="e5cf3-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
