---
title: Intune-Gerätebestand
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1281"
- "6700008"
ms.openlocfilehash: d59ee014a64de39d01837e90909619f30ec35e89
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434608"
---
# <a name="intune-device-inventory"></a><span data-ttu-id="501ce-102">Intune-Gerätebestand</span><span class="sxs-lookup"><span data-stu-id="501ce-102">Intune Device Inventory</span></span>

<span data-ttu-id="501ce-103">Das Blatt "Geräte" bietet dem Administrator einen Einblick in die in Intune verwalteten Geräte auf Gerätebasis.</span><span class="sxs-lookup"><span data-stu-id="501ce-103">The Devices blade provides the administrator insight into devices under management in Intune on a per device basis.</span></span> <span data-ttu-id="501ce-104">Die angezeigten Informationen umfassen: Hardware, entdeckte Anwendungen, Gerätecompliancestatus und Gerätekonfigurationsstatus.</span><span class="sxs-lookup"><span data-stu-id="501ce-104">The information shown includes: Hardware, Discovered applications, Device Compliance state, and Device Configuration state.</span></span>

<span data-ttu-id="501ce-105">Bestandsdaten für Hardware und entdeckte Anwendungen werden in einem siebentägigen Zyklus gesammelt.</span><span class="sxs-lookup"><span data-stu-id="501ce-105">Inventory data for hardware and discovered applications is collected on a seven-day cycle.</span></span> <span data-ttu-id="501ce-106">Die gemeldeten Anwendungen und spezifischen Elemente der Hardware unterscheiden sich je nach Betriebssystem des Geräts und je nachdem, ob das Gerät in Privat- oder Firmenbesitz ist.</span><span class="sxs-lookup"><span data-stu-id="501ce-106">The applications and specific elements of hardware reported differ depending on the device operating system and whether the device is personally or corporate owned.</span></span>

<span data-ttu-id="501ce-107">Weitere Informationen finden Sie unter [Anzeigen von Gerätedetails in Intune](https://docs.microsoft.com/intune/device-inventory).</span><span class="sxs-lookup"><span data-stu-id="501ce-107">For more information, see [See device details in Intune](https://docs.microsoft.com/intune/device-inventory).</span></span>

<span data-ttu-id="501ce-108">**Häufig gestellte Fragen**</span><span class="sxs-lookup"><span data-stu-id="501ce-108">**FAQ**</span></span>

<span data-ttu-id="501ce-109">F: Ich erhalte keine vollständige Bestandsliste der Anwendungen auf bei Intune registrierten Windows-Geräten.</span><span class="sxs-lookup"><span data-stu-id="501ce-109">Q: I am not receiving a full inventory list of applications present on Intune-enrolled Windows devices.</span></span> <span data-ttu-id="501ce-110">Warum nicht?</span><span class="sxs-lookup"><span data-stu-id="501ce-110">Why not?</span></span>

<span data-ttu-id="501ce-111">A: Gegenwärtig werden nur moderne Apps für als Unternehmensgeräte identifizierte Windows 10-PCs aufgeführt.</span><span class="sxs-lookup"><span data-stu-id="501ce-111">A: At this time, only modern apps are listed for Windows 10 PCs that are identified as corporate devices.</span></span> <span data-ttu-id="501ce-112">Intune sammelt keine Informationen über Win32-Anwendungen, die auf diesen Geräten installiert sind.</span><span class="sxs-lookup"><span data-stu-id="501ce-112">Intune doesn't collect information about Win32 apps installed on these devices.</span></span>

<span data-ttu-id="501ce-113">F: Warum werden Telefonnummern nicht von allen Geräten gesammelt?</span><span class="sxs-lookup"><span data-stu-id="501ce-113">Q: Why are phone numbers not collected from all devices?</span></span>

<span data-ttu-id="501ce-114">A: Telefone, die in Intune als Unternehmensgeräte kategorisiert sind, werden nicht mit ihrer vollständigen Telefonnummer identifiziert, wenn Sie z. B. einen Bestandsbericht für mobile Geräte ausführen.</span><span class="sxs-lookup"><span data-stu-id="501ce-114">A: Phones categorized as corporate devices in Intune are not identified with their full phone number when, for example, you run a mobile device inventory report.</span></span> <span data-ttu-id="501ce-115">Bring-Your-Own-Device-Telefonnummern werden immer teilweise mit Sternchen (\*\*\*\*) maskiert und zeigen nur die letzten vier Ziffern.</span><span class="sxs-lookup"><span data-stu-id="501ce-115">Bring-you-own-device phone numbers are always partially masked with asterisks (\*\*\*\*), and show only the last four digits.</span></span>