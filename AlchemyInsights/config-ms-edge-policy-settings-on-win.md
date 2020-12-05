---
title: Konfigurieren von Microsoft-Edge-Richtlinieneinstellungen unter Windows
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003845"
- "6894"
ms.openlocfilehash: 7f626152c3833638436dfe05e8dcd13fc86ef594
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576474"
---
# <a name="configure-microsoft-edge-policy-settings-on-windows"></a><span data-ttu-id="93e29-102">Konfigurieren von Microsoft-Edge-Richtlinieneinstellungen unter Windows</span><span class="sxs-lookup"><span data-stu-id="93e29-102">Configure Microsoft Edge policy settings on Windows</span></span>

<span data-ttu-id="93e29-103">Um Richtlinieneinstellungen und verwaltete Updates für Microsoft Edge zu konfigurieren, verwenden Sie Gruppenrichtlinienobjekte (Group Policy Objects, GPOs).</span><span class="sxs-lookup"><span data-stu-id="93e29-103">To configure policy settings and managed updates for Microsoft Edge, use Group Policy Objects (GPOs).</span></span> <span data-ttu-id="93e29-104">Sie können die Richtlinie auch über die Registrierung anbieten. Dies wäre für (1) Windows-Geräte geeignet, die einer Microsoft Active Directory-Domäne beigetreten sind, und für (2) Windows 10 pro-und Enterprise-Instanzen, die für die Geräteverwaltung in Microsoft InTune registriert sind.</span><span class="sxs-lookup"><span data-stu-id="93e29-104">You can also provision policy through the registry; this would be appropriate for (1) Windows devices joined to a Microsoft Active Directory domain and for (2) Windows 10 Pro and Enterprise instances enrolled for device management in Microsoft Intune.</span></span>

<span data-ttu-id="93e29-105">Führen Sie die folgenden Schritte aus, um Microsoft Edge mithilfe von GPOs zu konfigurieren:</span><span class="sxs-lookup"><span data-stu-id="93e29-105">To configure Microsoft Edge by using GPOs, do the following:</span></span>

1. <span data-ttu-id="93e29-106">Installieren Sie im zentralen Gruppenrichtlinien Speicher in Ihrer Active Directory Domäne oder im Ordner Richtlinien Definitions Vorlage auf einzelnen Computern alle administrativen Vorlagen, die Regeln und Einstellungen für Microsoft Edge hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="93e29-106">To the Group Policy Central Store in your Active Directory domain, or to the Policy Definition template folder on individual computers, install all administrative templates that add rules and settings for Microsoft Edge.</span></span>
2. <span data-ttu-id="93e29-107">Konfigurieren Sie die spezifischen Richtlinien, die Sie festlegen möchten.</span><span class="sxs-lookup"><span data-stu-id="93e29-107">Configure the specific policies you want to set.</span></span>

<span data-ttu-id="93e29-108">Weitere Informationen finden Sie unter [configure Microsoft Edge Policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span><span class="sxs-lookup"><span data-stu-id="93e29-108">To learn more, see [Configure Microsoft Edge policy settings on Windows](https://go.microsoft.com/fwlink/?linkid=2135024).</span></span>
