---
title: Verwenden der Microsoft Intune-Sicherheitsgrundsätze zum Konfigurieren von Windows 10-Geräten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/10/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8371"
- "9004622"
ms.openlocfilehash: b95454ec8ce8d0d69d1f55f7ce4adc596929e2de
ms.sourcegitcommit: 1b554c31d008492f9e6464f0249af0332212a3fc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50641620"
---
# <a name="use-the-microsoft-intune-security-baselines-for-configuring-windows-10-devices"></a><span data-ttu-id="ebc6b-102">Verwenden der Microsoft Intune-Sicherheitsgrundsätze zum Konfigurieren von Windows 10-Geräten</span><span class="sxs-lookup"><span data-stu-id="ebc6b-102">Use the Microsoft Intune security baselines for configuring Windows 10 devices</span></span>

<span data-ttu-id="ebc6b-103">Microsoft Intune-Sicherheitsgrundsätze helfen beim Schutz von Benutzern und Geräten.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-103">Intune security baselines help protect users and devices.</span></span> <span data-ttu-id="ebc6b-104">Sicherheitsgrundsätze sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den relevanten Sicherheitsteams empfohlen werden.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-104">Security baselines are Windows settings' pre-configured groups used to apply a known group of settings and default values recommended by the relevant security teams.</span></span> <span data-ttu-id="ebc6b-105">Durch Einrichten eines Profils der Sicherheitsgrundsätze in Microsoft Intune erstellen Sie eine Vorlage, die aus mehreren Gerätekonfigurationsprofilen besteht.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-105">By creating a security baseline profile in Intune, you create a template that consists of multiple device-configuration profiles.</span></span>

<span data-ttu-id="ebc6b-106">Wenn Sie Sicherheitsgrundsätze für Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die unter Windows 10 oder höheren Versionen ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-106">When you deploy security baselines to groups of users or devices, the settings are applied to devices that run on Windows 10 or later versions.</span></span> <span data-ttu-id="ebc6b-107">Die Microsoft MDM-Sicherheitsgrundsätze (Verwaltung mobiler Geräte) zum Beispiel (1) aktiviert automatisch BitLocker für Wechsellaufwerke, (2) fordert das Kennwort zum Entsperren eines Geräts an und (3) deaktiviert die Basisauthentifizierung.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-107">For example, the Microsoft mobile device management (MDM) security baseline automatically (1) enables BitLocker for removable drives, (2) requires the password for unlocking a device, and (3) disables basic authentication.</span></span> <span data-ttu-id="ebc6b-108">Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, können Sie die Grundsätze anpassen, um die gewünschten Einstellungen anzuwenden.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-108">When a default value doesn't work for your environment, you can customize the baseline to apply the settings you need.</span></span>

<span data-ttu-id="ebc6b-109">Sicherheitsgrundsätze helfen auch dabei, einen sicheren End-to-End-Workflow in Microsoft 365 zu etablieren.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-109">Security baselines also help establish an end-to-end secure workflow in Microsoft 365.</span></span> <span data-ttu-id="ebc6b-110">Im Folgenden sind einige Vorteile dieser Funktionalität aufgeführt:</span><span class="sxs-lookup"><span data-stu-id="ebc6b-110">The following are some benefits of this functionality:</span></span>
- <span data-ttu-id="ebc6b-111">Eine Sicherheitsgrundsatz umfasst bewährte Methoden und Empfehlungen für sicherheitsrelevante Einstellungen.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-111">A security baseline includes the best practices and recommendations for settings that affect security.</span></span> <span data-ttu-id="ebc6b-112">Da Microsoft Intune mit dem Windows-Sicherheitsteam zusammenarbeitet, das die Grundsätze für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf soliden Richtlinien und umfangreichen Erfahrungen.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-112">Because Intune partners with the Windows security team that creates baselines for group policies, these recommendations are based on solid guidance and extensive experience.</span></span>
- <span data-ttu-id="ebc6b-113">Wenn Sie neu bei Microsoft Intune sind und nicht wissen, wo Sie anfangen sollen, helfen Ihnen die Sicherheitsgrundsätze dabei, schnell ein sicheres Profil zu erstellen und bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-113">If you're new to Intune and unsure of where to start, then security baselines will help you quickly create and deploy a secure profile.</span></span>
- <span data-ttu-id="ebc6b-114">Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu Microsoft Intune für Verwaltungszwecke mit Sicherheitsgrundsätzen viel einfacher, da diese Sicherheitsgrundsätze in Microsoft Intune integriert sind und modernste Funktionen für die Verwaltung enthalten.</span><span class="sxs-lookup"><span data-stu-id="ebc6b-114">If you are currently using a group policy, then migrating to Intune for management purposes is much easier with security baselines, because these security baselines are built into Intune and include cutting-edge capabilities for management.</span></span>

<span data-ttu-id="ebc6b-115">Weitere Informationen finden Sie unter [Windows-Sicherheitsgrundsätze](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) und [Verwaltung mobiler Geräte (MDM)](https://docs.microsoft.com/windows/client-management/mdm/).</span><span class="sxs-lookup"><span data-stu-id="ebc6b-115">For more information, see [Windows security baselines](https://docs.microsoft.com/windows/security/threat-protection/windows-security-baselines) and [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/).</span></span>