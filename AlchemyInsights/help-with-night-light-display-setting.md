---
title: Hilfe für die Anzeigeeinstellungen des Nachtmodus
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9005578"
- "9930"
ms.openlocfilehash: db551db6edab7fca1cb465cf466575a2dbcd755e
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123079"
---
# <a name="help-with-the-night-light-display-setting"></a><span data-ttu-id="99af3-102">Hilfe für die Anzeigeeinstellungen des Nachtmodus</span><span class="sxs-lookup"><span data-stu-id="99af3-102">Help with the night light display setting</span></span>

<span data-ttu-id="99af3-103">Weitere Informationen über die Anzeigeeinstellungen des Nachtmodus finden Sie unter [Einrichten der Anzeige für die Nacht in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span><span class="sxs-lookup"><span data-stu-id="99af3-103">To learn more about night time display settings, see [Set your display for night time in Windows 10](https://support.microsoft.com/windows/set-your-display-for-night-time-in-windows-10-18fe903a-e0a1-8326-4c68-fd23d7aaf136).</span></span>

<span data-ttu-id="99af3-104">Wenn die Optionen für den Nachtmodus in den Einstellungen abgeblendet sind, überprüfen Sie Ihren Bildschirmtreiber:</span><span class="sxs-lookup"><span data-stu-id="99af3-104">If the night light options are grayed out in Settings, check your display driver:</span></span> 

1. <span data-ttu-id="99af3-105">Klicken Sie in das Suchfeld in Ihrer Taskleiste und geben Sie **Geräte-Manager** ein und wählen Sie dann **Geräte-Manager** in den Suchergebnissen aus.</span><span class="sxs-lookup"><span data-stu-id="99af3-105">Click the search box on your taskbar and type **Device Manager**, and then select **Device Manager** in the search results.</span></span>
1. <span data-ttu-id="99af3-106">Erweitern Sie **Bildschirm-Adapter**.</span><span class="sxs-lookup"><span data-stu-id="99af3-106">Expand **Display adapters**.</span></span> 

<span data-ttu-id="99af3-107">Leider ist die Nachtmodusfunktion nicht verfügbar, wenn Ihr Gerät einen DisplayLink-Treiber oder einen Standard-Bildschirmtreiber verwendet.</span><span class="sxs-lookup"><span data-stu-id="99af3-107">Unfortunately, the night light feature is not available if your device uses a DisplayLink driver or a Basic Display driver.</span></span>

<span data-ttu-id="99af3-108">Die Nachtmodusfunktion verwendet die neueste Grafiktechnologie, sodass Sie möglicherweise Ihren Bildschirmtreiber aktualisieren müssen:</span><span class="sxs-lookup"><span data-stu-id="99af3-108">The night light feature makes use of recent graphics technology, so you might need to update your display driver:</span></span>  

- <span data-ttu-id="99af3-109">Überprüfen Sie auf Updates, indem Sie zu **Start** > **Einstellungen** > **Update und Sicherheit** > **Windows Update** > **Nach Updates suchen** wechseln.</span><span class="sxs-lookup"><span data-stu-id="99af3-109">Check for updates by going to **Start** > **Settings** > **Update & Security** > **Windows Update** > **Check for Updates**.</span></span>  

<span data-ttu-id="99af3-110">ODER</span><span class="sxs-lookup"><span data-stu-id="99af3-110">OR</span></span>

- <span data-ttu-id="99af3-111">Besuchen Sie die Support-Website Ihres Hardwareherstellers, um die neuesten Bildschirmtreiber manuell herunterzuladen und zu installieren.</span><span class="sxs-lookup"><span data-stu-id="99af3-111">Visit your hardware manufacturer's support website to manually download and install the latest display drivers.</span></span>

## <a name="reset-night-light-in-the-registry"></a><span data-ttu-id="99af3-112">Setzen Sie den Nachtmodus in der Registrierung zurück.</span><span class="sxs-lookup"><span data-stu-id="99af3-112">Reset night light in the registry</span></span>

<span data-ttu-id="99af3-113">Wenn die Aktualisierung Ihres Anzeigetreibers nicht funktioniert hat, müssen Sie möglicherweise den Nachtmodus in der Registrierung zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="99af3-113">If updating your display driver didn't work, you might need to reset night light in the registry.</span></span>  

<span data-ttu-id="99af3-114">**Vorsicht**: Dieser Problembehandlungsschritt wird nur fortgeschrittenen Benutzer empfohlen.</span><span class="sxs-lookup"><span data-stu-id="99af3-114">**Caution:** This troubleshooting step is recommended only for advanced users.</span></span> <span data-ttu-id="99af3-115">Durch eine fehlerhafte Bearbeitung der Registrierung können schwerwiegende Probleme verursacht werden.</span><span class="sxs-lookup"><span data-stu-id="99af3-115">Serious problems can occur if you modify the registry incorrectly.</span></span> <span data-ttu-id="99af3-116">Sichern Sie für zusätzlichen Schutz die Registrierung, bevor Sie diese ändern, damit sie bei Problemen wiederhergestellt werden kann.</span><span class="sxs-lookup"><span data-stu-id="99af3-116">For added protection, back up the registry before you modify it so  you can restore it if problems occur.</span></span>

1. <span data-ttu-id="99af3-117">Geben Sie im Suchfeld **regedit** ein, und wählen Sie den **Registrierungs-Editor** in den Suchergebnissen aus.</span><span class="sxs-lookup"><span data-stu-id="99af3-117">In the search box, type **regedit**, and then select **Registry Editor** in the search results.</span></span>

1. <span data-ttu-id="99af3-118">Navigieren Sie zu folgendem Registrierungsschlüssel:</span><span class="sxs-lookup"><span data-stu-id="99af3-118">Go to the following registry key:</span></span> 

    <span data-ttu-id="99af3-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span><span class="sxs-lookup"><span data-stu-id="99af3-119">HKEY_CURRENT_USER\Software\Microsoft\Windows\CurrentVersion\CloudStore\Store\Cache\DefaultAccount</span></span>

1. <span data-ttu-id="99af3-120">Exportieren und Löschen Sie danach den folgenden Eintrag subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span><span class="sxs-lookup"><span data-stu-id="99af3-120">Export and then delete the following subkey:$$windows.data.bluelightreduction.bluelightreductionstate</span></span>

1. <span data-ttu-id="99af3-121">Exportieren und Löschen Sie danach den folgenden Eintrag subkey:$$windows.data.bluelightreduction.settings</span><span class="sxs-lookup"><span data-stu-id="99af3-121">Export and then delete the following subkey:$$windows.data.bluelightreduction.settings</span></span>

1. <span data-ttu-id="99af3-122">Starten Sie Windows neu und verifizieren Sie, dass die Optionen für den Nachtmodus verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="99af3-122">Restart Windows and verify if the night light options are available.</span></span>


