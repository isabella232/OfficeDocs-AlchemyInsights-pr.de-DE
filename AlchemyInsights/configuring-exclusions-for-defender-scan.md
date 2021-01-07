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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768490"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="61fe1-102">Konfigurieren von Ausschlüssen für den Microsoft Defender ATP-Scan</span><span class="sxs-lookup"><span data-stu-id="61fe1-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="61fe1-103">Im Allgemeinen können Sie bestimmte Dateierweiterungen und Ordnerspeicherorte von Microsoft Defender ATP-Scans ausschließen.</span><span class="sxs-lookup"><span data-stu-id="61fe1-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="61fe1-104">Sie können auch Ausschlüsse für Dateien konfigurieren, die von bestimmten Prozessen geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="61fe1-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="61fe1-105">Weitere Informationen finden Sie unter [Konfigurieren und Überprüfen von Ausschlüssen basierend auf Dateierweiterung und Ordnerspeicherorten](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) sowie [Konfigurieren von Ausschlüssen Dateien, die von bestimmten Prozessen geöffnet wurden](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="61fe1-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="61fe1-106">Um Ausschlüsse für **Windows Server 2016 und 2019** zu konfigurieren, lesen Sie [Konfigurieren von Microsoft Defender Antivirus-Ausschlüssen unter Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span><span class="sxs-lookup"><span data-stu-id="61fe1-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="61fe1-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="61fe1-107">**Mac**</span></span>

<span data-ttu-id="61fe1-108">Details zu unterstützten Ausschlusstypen und zum Konfigurieren einer Liste von Ausschlüssen für Mac finden Sie unter [Unterstützte Ausschlusstypen](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) und [Konfigurieren der Liste der Ausschlüsse](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span><span class="sxs-lookup"><span data-stu-id="61fe1-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="61fe1-109">**Hinweis** Sie können Ausschlusslisten auch mithilfe der EICAR-Testdatei validieren.</span><span class="sxs-lookup"><span data-stu-id="61fe1-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="61fe1-110">Weitere Informationen finden Sie unter [Validieren von Ausschlusslisten mit der EICAR-Testdatei](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="61fe1-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="61fe1-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="61fe1-111">**Linux**</span></span>

<span data-ttu-id="61fe1-112">Details zu unterstützten Ausschlusstypen und zum Konfigurieren einer Liste von Ausschlüssen für Linux finden Sie unter [Unterstützte Ausschlusstypen](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) sowie [Konfigurieren und Validieren von Ausschlüssen für Microsoft Defender ATP für Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span><span class="sxs-lookup"><span data-stu-id="61fe1-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="61fe1-113">**Hinweis** Sie können Ausschlusslisten auch mithilfe der EICAR-Testdatei validieren.</span><span class="sxs-lookup"><span data-stu-id="61fe1-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="61fe1-114">Weitere Informationen finden Sie unter [Validieren von Ausschlusslisten mit der EICAR-Testdatei](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span><span class="sxs-lookup"><span data-stu-id="61fe1-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 