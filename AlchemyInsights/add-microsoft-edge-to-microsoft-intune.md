---
title: Hinzufügen von Microsoft Edge zu Microsoft Intune
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/10/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8240"
- "9004604"
ms.openlocfilehash: d56c65910d1c2170d3e0ce9676e913663701db96
ms.sourcegitcommit: 03378c78eadac5d950802dcbacc328bca3314032
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 02/10/2021
ms.locfileid: "50177998"
---
# <a name="add-microsoft-edge-to-microsoft-intune"></a><span data-ttu-id="7c436-102">Hinzufügen von Microsoft Edge zu Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="7c436-102">Add Microsoft Edge to Microsoft Intune</span></span>

<span data-ttu-id="7c436-103">Um Microsoft Edge für Windows 10 bereitstellen, konfigurieren, überwachen und schützen zu können, müssen Sie es zunächst zu Microsoft Intune hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="7c436-103">To be able to deploy, configure, monitor, and protect Microsoft Edge for Windows 10, you must first add it to Microsoft Intune.</span></span>

> [!IMPORTANT]
- <span data-ttu-id="7c436-104">Intune unterstützt Microsoft Edge 77 und spätere Versionen.</span><span class="sxs-lookup"><span data-stu-id="7c436-104">Intune supports Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="7c436-105">Intune erkennt alle bereits vorhandenen Installationen von Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="7c436-105">Intune will detect any pre-existing installations of Microsoft Edge.</span></span>
- <span data-ttu-id="7c436-106">Wenn Microsoft Edge im Benutzerkontext installiert wird, überschreibt eine Systeminstallation die Installation im Benutzerkontext.</span><span class="sxs-lookup"><span data-stu-id="7c436-106">If Microsoft Edge is installed in user context, a system installation will overwrite the installation in user context.</span></span>
- <span data-ttu-id="7c436-107">Wird Microsoft Edge im Systemkontext installiert, wird der Installationserfolg gemeldet.</span><span class="sxs-lookup"><span data-stu-id="7c436-107">If Microsoft Edge is installed in system context, the installation success will be reported.</span></span>
- <span data-ttu-id="7c436-108">Vorinstallierte Microsoft Edge 77 und spätere Versionen werden für alle Kanäle im Benutzerkontext mit dem im Systemkontext installierten Microsoft Edge überschrieben.</span><span class="sxs-lookup"><span data-stu-id="7c436-108">Pre-installed Microsoft Edge 77 and later versions, for all channels in user context, will be overwritten with Microsoft Edge installed in system context.</span></span>

<span data-ttu-id="7c436-109">**Voraussetzungen**</span><span class="sxs-lookup"><span data-stu-id="7c436-109">**Prerequisite**</span></span>

<span data-ttu-id="7c436-110">Windows 10, Version 1709 oder höher</span><span class="sxs-lookup"><span data-stu-id="7c436-110">Windows 10 version 1709 or later versions</span></span>

<span data-ttu-id="7c436-111">**Schritte zum Hinzufügen von Microsoft Edge zu Intune**</span><span class="sxs-lookup"><span data-stu-id="7c436-111">**Steps to add Edge to Intune**</span></span>

1. <span data-ttu-id="7c436-112">[Konfigurieren Sie die App in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-112">[Configure the app in Intune](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
2. <span data-ttu-id="7c436-113">[Konfigurieren Sie die App-Informationen](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-113">[Configure the app information](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
3. <span data-ttu-id="7c436-114">[Konfigurieren Sie die App-Einstellungen](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-114">[Configure the app settings](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
4. <span data-ttu-id="7c436-115">[Wählen Sie die Bereichs-Tags aus (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-115">[Select the scope tags (optional)](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>
5. <span data-ttu-id="7c436-116">[Fügen Sie die App hinzu](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-116">[Add the app](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>

<span data-ttu-id="7c436-117">Weitere Hilfe finden Sie unter [Problembehandlung](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span><span class="sxs-lookup"><span data-stu-id="7c436-117">For more help, see [Troubleshooting](https://docs.microsoft.com/mem/intune/apps/apps-windows-edge).</span></span>




