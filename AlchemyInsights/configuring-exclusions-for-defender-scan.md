---
title: Konfigurieren von Ausschlüssen für den Microsoft Defender ATP-Scan
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543684"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="904d4-102">Konfigurieren von Ausschlüssen für den Microsoft Defender ATP-Scan</span><span class="sxs-lookup"><span data-stu-id="904d4-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="904d4-103">Im Allgemeinen können Sie bestimmte Dateierweiterungen und Ordnerspeicherorte von Microsoft Defender ATP-Scans ausschließen.</span><span class="sxs-lookup"><span data-stu-id="904d4-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="904d4-104">Sie können auch Ausschlüsse für Dateien konfigurieren, die von bestimmten Prozessen geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="904d4-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="904d4-105">Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen basierend auf Dateierweiterung und Ordnerspeicherorten](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) sowie [Konfigurieren von Ausschlüssen Dateien, die von bestimmten Prozessen geöffnet wurden](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="904d4-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="904d4-106">Um Ausschlüsse für **Windows Server 2016 und 2019** zu konfigurieren, lesen Sie [Konfigurieren von Microsoft Defender Antivirus-Ausschlüssen unter Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="904d4-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="904d4-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="904d4-107">**Mac**</span></span>

<span data-ttu-id="904d4-108">Details zu unterstützten Ausschlusstypen und zum Konfigurieren einer Liste von Ausschlüssen für Mac finden Sie unter [Unterstützte Ausschlusstypen](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) und [Konfigurieren der Liste der Ausschlüsse](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="904d4-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="904d4-109">**Hinweis** Sie können Ausschlusslisten auch mithilfe der EICAR-Testdatei validieren.</span><span class="sxs-lookup"><span data-stu-id="904d4-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="904d4-110">Weitere Informationen finden Sie unter [Validieren von Ausschlusslisten mit der EICAR-Testdatei](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="904d4-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="904d4-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="904d4-111">**Linux**</span></span>

<span data-ttu-id="904d4-112">Details zu unterstützten Ausschlusstypen und zum Konfigurieren einer Liste von Ausschlüssen für Linux finden Sie unter [Unterstützte Ausschlusstypen](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) sowie [Konfigurieren und Validieren von Ausschlüssen für Microsoft Defender ATP für Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="904d4-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="904d4-113">**Hinweis** Sie können Ausschlusslisten auch mithilfe der EICAR-Testdatei validieren.</span><span class="sxs-lookup"><span data-stu-id="904d4-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="904d4-114">Weitere Informationen finden Sie unter [Validieren von Ausschlusslisten mit der EICAR-Testdatei](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="904d4-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 