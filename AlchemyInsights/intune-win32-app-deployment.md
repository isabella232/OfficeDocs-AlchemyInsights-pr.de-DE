---
title: Intune Win32 App-Bereitstellung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366525"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="3506b-102">Intune Win32 App-Bereitstellung</span><span class="sxs-lookup"><span data-stu-id="3506b-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="3506b-103">Mit Microsoft Intune können Win32-Anwendungen, einschließlich aber nicht beschränkt auf MSI und .EXE, auf Windows 10-Geräten bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="3506b-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="3506b-104">Für den verwendeten Bereitstellungsmechanismus muss die Intune-Verwaltungserweiterung (IME) auf dem Zielgerät installiert sein.</span><span class="sxs-lookup"><span data-stu-id="3506b-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="3506b-105">Die IME wird automatisch installiert, wenn ein PowerShell-Skript ausgeführt wird, oder eine Win32-Anwendung für einen Benutzer/auf ein Benutzergerät bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="3506b-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="3506b-106">Es gibt außerdem eine Reihe an Voraussetzungen, die für die Bereitstellung von Win32-Apps erfüllt werden müssen. Dazu gehören:</span><span class="sxs-lookup"><span data-stu-id="3506b-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="3506b-107">Unterstützte Plattformen: Windows 10 Version 1607 oder später (Enterprise, Pro, und Education-Versionen).</span><span class="sxs-lookup"><span data-stu-id="3506b-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="3506b-108">Unterstützte Architektur: x86 und x64.</span><span class="sxs-lookup"><span data-stu-id="3506b-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="3506b-109">Geräteverwaltung: ADD eingebunden und automatisch registriert (darunter Hybriddomäne eingebunden und Gruppenrichtlinie automatisch registriert).</span><span class="sxs-lookup"><span data-stu-id="3506b-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="3506b-110">Format des Anwendungspakets: Die .**intunewin** -Datei wird von dem [Tool zur Vorbereitung von Microsoft Win32-Inhalten](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare) vorbereitet.</span><span class="sxs-lookup"><span data-stu-id="3506b-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="3506b-111">Einschränkungen:</span><span class="sxs-lookup"><span data-stu-id="3506b-111">Limitations:</span></span>
    - <span data-ttu-id="3506b-112">Maximale Größe: 8 GB.</span><span class="sxs-lookup"><span data-stu-id="3506b-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="3506b-113">Nicht unterstützte Architektur: ARMs.</span><span class="sxs-lookup"><span data-stu-id="3506b-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="3506b-114">Lesen Sie das Dokument „[Eine Win32-App in Microsoft Intune hinzufügen, zuweisen und überwachen](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)“, um weitere Informationen zu diesen Schritten zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="3506b-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="3506b-115">Genauere Informationen zur Problembehandlung der Anwendungsbereitstellung auf Windows, einschließlich der Bereitstellung von Win32-Apps, erhalten Sie in den folgenden Dokumenten</span><span class="sxs-lookup"><span data-stu-id="3506b-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="3506b-116">Behandeln von Problemen bei der App-Installation</span><span class="sxs-lookup"><span data-stu-id="3506b-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="3506b-117">Problembehandlung bei Win32-Apps</span><span class="sxs-lookup"><span data-stu-id="3506b-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)