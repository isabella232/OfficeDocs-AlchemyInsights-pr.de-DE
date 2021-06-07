---
title: Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9006500"
- "11142"
ms.openlocfilehash: 88525fccd6dcde0cb3949e348d1f2a7df3ee7ce7
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/06/2021
ms.locfileid: "52783188"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a><span data-ttu-id="7545e-102">Verwenden Microsoft Intune Sicherheitsgrundwerte zum Konfigurieren Windows 10 Geräten</span><span class="sxs-lookup"><span data-stu-id="7545e-102">Use Microsoft Intune security baselines to configure Windows 10 devices</span></span>

<span data-ttu-id="7545e-103">Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten.</span><span class="sxs-lookup"><span data-stu-id="7545e-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="7545e-104">Sicherheitsgrundwerte sind Windows vorkonfigurierte Gruppen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den entsprechenden Sicherheitsteams empfohlen werden.</span><span class="sxs-lookup"><span data-stu-id="7545e-104">Security baselines are Windows settings pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="7545e-105">Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.</span><span class="sxs-lookup"><span data-stu-id="7545e-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="7545e-106">Wenn Sie Sicherheitsgrundwerte für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die auf Windows 10 oder höher ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="7545e-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later.</span></span> <span data-ttu-id="7545e-107">Beispielsweise aktiviert die Microsoft Mobile Device Management (MDM)-Sicherheitsgrundlinie automatisch BitLocker für Wechseldatenträger, erfordert das Kennwort zum Entsperren eines Geräts und deaktiviert die Standardauthentifizierung.</span><span class="sxs-lookup"><span data-stu-id="7545e-107">For example, the Microsoft mobile device management (MDM) security baseline automatically enables BitLocker for removable drives, requires the password for unlocking a device, and disables basic authentication.</span></span> <span data-ttu-id="7545e-108">Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="7545e-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="7545e-109">Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren.</span><span class="sxs-lookup"><span data-stu-id="7545e-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="7545e-110">Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="7545e-110">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="7545e-111">Intune arbeitet mit dem Windows Sicherheitsteam zusammen, das Basispläne für Gruppenrichtlinien erstellt, sodass diese Empfehlungen auf soliden Anleitungen und umfangreicher Erfahrung basieren.</span><span class="sxs-lookup"><span data-stu-id="7545e-111">Intune partners with the Windows security team that creates baselines for group policies, so these recommendations are based on solid guidance and extensive experience.</span></span>

<span data-ttu-id="7545e-112">Wenn Sie noch nicht mit Intune vertraut sind und sich nicht sicher sind, wo Sie beginnen sollten, helfen Ihnen Sicherheitsgrundwerte, schnell ein sicheres Profil zu erstellen und bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="7545e-112">If you're new to Intune and unsure of where to start, security baselines help you quickly create and deploy a secure profile.</span></span> <span data-ttu-id="7545e-113">Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Intune zu Verwaltungszwecken mit Sicherheitsgrundwerten viel einfacher, da sie in Intune integriert sind und moderne Verwaltungsfunktionen enthalten.</span><span class="sxs-lookup"><span data-stu-id="7545e-113">If you currently use a group policy, migrating to Intune for management purposes is much easier with security baselines because they are built into Intune and include cutting-edge management capabilities.</span></span>

<span data-ttu-id="7545e-114">Weitere Informationen finden Sie [unter Windows Sicherheitsgrundwerte](/windows/security/threat-protection/windows-security-baselines) und [verwaltung mobiler Geräte.](/windows/client-management/mdm/)</span><span class="sxs-lookup"><span data-stu-id="7545e-114">To learn more, see [Windows security baselines](/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](/windows/client-management/mdm/).</span></span>

