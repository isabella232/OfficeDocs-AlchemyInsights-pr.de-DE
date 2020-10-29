---
title: Dateien bei Bedarf
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 4e3da81ee048c6257e05b998c0f457fa433738fd
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791293"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="9c430-102">OneDrive-Dateien bei Bedarf konfigurieren</span><span class="sxs-lookup"><span data-stu-id="9c430-102">Configure Files On-Demand</span></span>

<span data-ttu-id="9c430-103">OneDrive-Dateien bei Bedarf benötigt [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (Version 1709 oder höher) oder Windows Server 2019 und OneDrive Build 17.3.7064.1005 oder höher.</span><span class="sxs-lookup"><span data-stu-id="9c430-103">OneDrive Files On-Demand requires [Windows 10 Fall Creators Update](https://go.microsoft.com/fwlink/p/?linkid=859040) (version 1709 or later) or Windows Server 2019 and OneDrive build 17.3.7064.1005 or later.</span></span>

<span data-ttu-id="9c430-104">Mit OneDrive-Dateien bei Bedarf können Sie auf alle Ihre Dateien in OneDrive zugreifen, ohne alle herunterladen und Speicherplatz auf Ihrem Gerät nutzen zu müssen.</span><span class="sxs-lookup"><span data-stu-id="9c430-104">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="9c430-105">So konfigurieren Sie die Dateien bei Bedarf auf Ihrem PC:</span><span class="sxs-lookup"><span data-stu-id="9c430-105">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="9c430-106">Wählen Sie das weiße oder blaue **OneDrive** Cloudsymbol im Benachrichtigungsbereich der Windows-Taskleiste aus.</span><span class="sxs-lookup"><span data-stu-id="9c430-106">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="9c430-107">Wählen Sie **Hilfe & Einstellungen** Zahnradsymbol > **Einstellungen** .</span><span class="sxs-lookup"><span data-stu-id="9c430-107">Select the **Help & Settings** gear icon > **Settings** .</span></span>
2. <span data-ttu-id="9c430-108">Aktivieren Sie auf der Registerkarte **Einstellungen** das Kontrollkästchen **Platz sparen und Dateien erst bei Verwendung herunterladen** .</span><span class="sxs-lookup"><span data-stu-id="9c430-108">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="9c430-109">Sie können Dateien bei Bedarf auch mithilfe der Registrierung konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="9c430-109">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="9c430-110">Wenn Sie diese Einstellung deaktivieren, weisen Windows 10-Benutzer das gleiche Synchronisierungsverhalten wie Benutzer der früheren Versionen von Windows auf, und sie können "Dateien bei Bedarf" nicht aktivieren.</span><span class="sxs-lookup"><span data-stu-id="9c430-110">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="9c430-111">Wenn Sie diese Einstellung nicht konfigurieren, können die Benutzer „Dateien bei Bedarf“ aktivieren oder deaktivieren.</span><span class="sxs-lookup"><span data-stu-id="9c430-111">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="9c430-112">Durch Aktivieren dieser Richtlinie wird der folgende Registrierungsschlüsselwert auf 1 festgelegt.</span><span class="sxs-lookup"><span data-stu-id="9c430-112">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="9c430-113">Das Deaktivieren dieser Richtlinie setzt den folgenden Registrierungsschlüsselwert auf 0.</span><span class="sxs-lookup"><span data-stu-id="9c430-113">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="9c430-114">Wenn die Dateien bei Bedarf-Option in „Einstellungen“ nicht angezeigt wird, stellen Sie sicher, dass der Starttyp des Dienstes „Windows-Clouddateien-Filter-Treiber“ auf 2 (AUTO_START) festgelegt ist.</span><span class="sxs-lookup"><span data-stu-id="9c430-114">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="9c430-115">Das Aktivieren dieses Features setzt den folgende Registrierungsschlüsselwert auf 2.</span><span class="sxs-lookup"><span data-stu-id="9c430-115">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`