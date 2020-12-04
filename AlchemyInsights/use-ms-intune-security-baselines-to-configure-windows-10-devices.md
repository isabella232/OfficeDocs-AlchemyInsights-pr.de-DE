---
title: Verwenden von Microsoft InTune-Sicherheitsbasislinien zum Konfigurieren von Windows 10-Geräten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571828"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="1dbd3-102">Verwenden von Microsoft InTune-Sicherheitsbasislinien zum Konfigurieren von Windows 10-Geräten</span><span class="sxs-lookup"><span data-stu-id="1dbd3-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="1dbd3-103">InTune-Sicherheitsbasislinien tragen zum Schutz von Benutzern und Geräten bei.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="1dbd3-104">Sicherheitsbasislinien sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den entsprechenden Sicherheitsteams empfohlen werden.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="1dbd3-105">Durch das Erstellen eines Sicherheitsbasis Profils in InTune erstellen Sie eine Vorlage, die aus mehreren Geräte Konfigurationsprofilen besteht.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="1dbd3-106">Wenn Sie Sicherheitsbasislinien in Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die unter Windows 10 oder höher ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="1dbd3-107">Beispielsweise aktiviert die MDM-Sicherheitsbasislinie automatisch (1) BitLocker für Wechseldatenträger, (2) erfordert das Kennwort für das Entsperren eines Geräts, und (3) deaktiviert die Standardauthentifizierung.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-107">For example, MDM Security Baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="1dbd3-108">Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, passen Sie die Basislinie an, um die erforderlichen Einstellungen anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-108">When a default value doesn't work for your environment, customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="1dbd3-109">Sicherheitsbasislinien helfen außerdem bei der Einrichtung eines End-to-End-sicheren Workflows in Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="1dbd3-110">Im folgenden finden Sie einige Vorteile:</span><span class="sxs-lookup"><span data-stu-id="1dbd3-110">The following are some benefits of this:</span></span>

- <span data-ttu-id="1dbd3-111">Eine Sicherheitsbasislinie enthält die bewährten Methoden und Empfehlungen für Einstellungen, die sich auf die Sicherheit auswirken.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="1dbd3-112">Da InTune mit dem Windows-Sicherheitsteam arbeitet, das Basispläne für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf fundierten Anleitungen und umfangreichen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="1dbd3-113">Wenn Sie neu in InTune sind und sich nicht sicher sind, wo Sie beginnen sollen, können Sicherheitsbasislinien Ihnen helfen, ein sicheres Profil schnell zu erstellen und bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="1dbd3-114">Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu InTune für Verwaltungszwecke mit Sicherheitsbasislinien wesentlich einfacher, da Sie in InTune integriert sind und innovative Funktionen für die Verwaltung umfassen.</span><span class="sxs-lookup"><span data-stu-id="1dbd3-114">If you currently use a group policy, then migrating to Intune for management purposes is much easier with security baselines, because they are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="1dbd3-115">Weitere Informationen finden Sie unter [Windows-Sicherheitsbasislinien](https://go.microsoft.com/fwlink/?linkid=2141503) und [Verwaltung mobiler Geräte](https://go.microsoft.com/fwlink/?linkid=2141701).</span><span class="sxs-lookup"><span data-stu-id="1dbd3-115">To learn more, see [Windows security baselines](https://go.microsoft.com/fwlink/?linkid=2141503) and [Mobile device management](https://go.microsoft.com/fwlink/?linkid=2141701).</span></span>