---
title: EndPoint Manager – Sicherheitsbasispläne
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51408760"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="c1710-102">EndPoint Manager – Sicherheitsbasispläne</span><span class="sxs-lookup"><span data-stu-id="c1710-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="c1710-103">Sicherheitsbasispläne sind vorkonfigurierte Gruppen von Windows-Einstellungen, mit denen Sie die von den entsprechenden Sicherheitsteams empfohlenen Sicherheitseinstellungen anwenden können.</span><span class="sxs-lookup"><span data-stu-id="c1710-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="c1710-104">Diese Basispläne können angepasst werden, um nur die gewünschten Einstellungen und Werte zu liefern.</span><span class="sxs-lookup"><span data-stu-id="c1710-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="c1710-105">Weitere Informationen zu Sicherheitsbasispläne finden Sie unter [Verwenden von Sicherheitsbasispläne zum Konfigurieren von Windows 10-Geräten in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c1710-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="c1710-106">Derzeit gibt es Basispläne für diese Produkte:</span><span class="sxs-lookup"><span data-stu-id="c1710-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="c1710-107">Windows MDM-Sicherheitseinstellungen</span><span class="sxs-lookup"><span data-stu-id="c1710-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="c1710-108">Microsoft Defender für EndPoint Security</span><span class="sxs-lookup"><span data-stu-id="c1710-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="c1710-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c1710-109">Microsoft Edge</span></span>

<span data-ttu-id="c1710-110">Jede der Basispläne wird regelmäßig aktualisiert und in inkrementellen Versionen veröffentlicht.</span><span class="sxs-lookup"><span data-stu-id="c1710-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="c1710-111">In jeder Version werden Einstellungen zur vorherigen Version hinzugefügt und/oder entfernt, um sicherzustellen, dass der Basisplan den aktuellen Richtlinien entspricht.</span><span class="sxs-lookup"><span data-stu-id="c1710-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="c1710-112">Über die Security Basisplan-Konsole in Endpoint Security können verschiedene Versionen verglichen werden, indem die Änderungen von Version zu Version sichtbar gemacht werden.</span><span class="sxs-lookup"><span data-stu-id="c1710-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="c1710-113">Anleitungen zum effektivsten Ändern der bereitgestellten Basisplan-Version finden Sie unter [Verwalten von Sicherheitsbasisplan-Profilen in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="c1710-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="c1710-114">Nach der Bereitstellung eines Sicherheitsbasisplans können Sie den Bereitstellungsstatus überwachen und die Einstellungen geräteweise überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c1710-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="c1710-115">**Hinweis:** Es kann bis zu 24 Stunden dauern, bis die Berichtsdaten für Basispläne von der ersten Bereitstellung auf einem Gerät bis zu 6 Stunden für weitere Aktualisierungen angezeigt werden.</span><span class="sxs-lookup"><span data-stu-id="c1710-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="c1710-116">Die häufigste Ursache dafür, dass eine Grundeinstellung nicht angewendet wird, ist, dass dieselbe Einstellung in einem anderen Profil verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="c1710-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="c1710-117">Dieses Szenario kann für ein bestimmtes Gerät untersucht werden, indem dieses Gerät im Knoten Gerätestatus des Security Basisplanprofils ausgewählt wird.</span><span class="sxs-lookup"><span data-stu-id="c1710-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="c1710-118">Weitere Informationen finden Sie unter [Lösen von Konflikten für Sicherheitsbasispläne](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c1710-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>