---
title: Intune-WLAN-Profile
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
- "1548"
- "9000076"
ms.openlocfilehash: afc8142a635b8a9d715eb4325b570be20ad26645
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696260"
---
# <a name="intune-wi-fi-profiles"></a><span data-ttu-id="8d249-102">Intune-WLAN-Profile</span><span class="sxs-lookup"><span data-stu-id="8d249-102">Intune Wi-Fi profiles</span></span>

<span data-ttu-id="8d249-103">Die erfolgreiche Implementierung von WLAN-Konnektivität für MDM-Clients hängt von einem korrekt bereitgestellten Profil ab, das die Anforderungen der WLAN-Infrastruktur des Unternehmens widerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="8d249-103">Successful implementation of Wi-Fi connectivity for MDM clients depends on a correctly deployed profile that reflects the requirements of the corporate Wi-Fi infrastructure.</span></span> <span data-ttu-id="8d249-104">Informationen zum Überprüfen der entsprechenden Einstellungen für die Clientplattformen, die Sie untersuchen, finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="8d249-104">To review the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="8d249-105">Hinzufügen von WLAN-Einstellungen für Geräte, die Android in Microsoft Intune ausführen</span><span class="sxs-lookup"><span data-stu-id="8d249-105">Add Wi-Fi settings for devices running Android in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android)

[<span data-ttu-id="8d249-106">Hinzufügen von WLAN-Einstellungen für Android Enterprise-dedizierte und vollständig verwaltete Geräte in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8d249-106">Add Wi-Fi settings for Android Enterprise dedicated and fully managed devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-android-enterprise)

[<span data-ttu-id="8d249-107">Hinzufügen von WLAN-Einstellungen für iOS- und iPadOS-Geräte in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="8d249-107">Add Wi-Fi settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-ios)

[<span data-ttu-id="8d249-108">Hinzufügen von WLAN-Einstellungen für Windows 10-Geräte und Geräte mit einer höheren Windows-Version in Intune</span><span class="sxs-lookup"><span data-stu-id="8d249-108">Add Wi-Fi settings for Windows 10 and later devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-windows)

[<span data-ttu-id="8d249-109">Importieren von WLAN-Einstellungen für Windows-Geräte in Intune</span><span class="sxs-lookup"><span data-stu-id="8d249-109">Import Wi-Fi settings for Windows devices in Intune</span></span>](https://docs.microsoft.com/intune/wi-fi-settings-import-windows-8-1)

<span data-ttu-id="8d249-110">**Häufig auftretende Probleme**</span><span class="sxs-lookup"><span data-stu-id="8d249-110">**Common Issues**</span></span>

<span data-ttu-id="8d249-111">**Ich stellen ein WLAN-Profil bereit, das von einem bereitgestellten Zertifikat abhängig ist, das im WLAN-Profil angegeben ist. Die Konfigurationsprofile weisen jedoch einen Fehlerstatus auf.**</span><span class="sxs-lookup"><span data-stu-id="8d249-111">**I'm deploying a Wi-Fi profile that is dependent on a deployed certificate specified in the Wi-Fi profile. However, the configuration profiles are showing an error status.**</span></span>

<span data-ttu-id="8d249-112">Überprüfen Sie, ob Ihr Gerät das Zertifikat erhalten hat.</span><span class="sxs-lookup"><span data-stu-id="8d249-112">Check that your device received the certificate.</span></span>

1. <span data-ttu-id="8d249-113">Wechseln Sie in Intune zu **Alle Geräte**, und wählen Sie das Gerät > **Gerätekonfiguration** aus.</span><span class="sxs-lookup"><span data-stu-id="8d249-113">In Intune, go to **All Devices** and select the device > **Device configuration**.</span></span>

2. <span data-ttu-id="8d249-114">Überprüfen Sie, ob alle erwarteten Profile aufgeführt sind und einen erfolgreichen Zustand aufweisen.</span><span class="sxs-lookup"><span data-stu-id="8d249-114">Check that all expected profiles are listed and in a successful state.</span></span>

3. <span data-ttu-id="8d249-115">Wenn Sie bei einem Android-Profil Zwischenzertifikate in Ihrer Zertifikatkette besitzen, müssen Sie sicherstellen, dass diese auf Android-Geräten bereitgestellt sind.</span><span class="sxs-lookup"><span data-stu-id="8d249-115">For an Android profile, if you have intermediate certificates in your certificate chain, make sure they are deployed to Android devices.</span></span>

    <span data-ttu-id="8d249-116">Um den Zertifikatstatus zu überprüfen, wechseln Sie zu **Gerätekonfiguration** > **Profile** > **Android-Zwischenzertifizierungsstelle** > **Eigenschaften** > **vertrauenswürdiges Zertifikat**.</span><span class="sxs-lookup"><span data-stu-id="8d249-116">To check the certificate status, go to **Device configuration** > **Profiles** > **Android intermediate CA** > **Properties** > **Trusted Certificate**.</span></span>

<span data-ttu-id="8d249-117">Wenn weiterhin Fehler angezeigt werden, lesen Sie die Abschnitte zur Verfahren und zur Problembehandlung.</span><span class="sxs-lookup"><span data-stu-id="8d249-117">If you continue to see errors, review the procedures and troubleshooting sections.</span></span> <span data-ttu-id="8d249-118">Weitere Informationen finden Sie unter [Übersicht für die Problembehandlung von SCEP-Zertifikatprofilen mit Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="8d249-118">For more info, see [Overview for troubleshooting SCEP certificate profiles with Microsoft Intune](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune).</span></span>

<span data-ttu-id="8d249-119">**Ich habe ein WLAN-Profil auf einem Gerät bereitgestellt. Intune zeigt an, dass dies erfolgreich war, aber das Gerät verbindet sich nicht mit dem WLAN.**</span><span class="sxs-lookup"><span data-stu-id="8d249-119">**I deployed a Wi-Fi profile to a device. Intune is showing that it was successful, but the device is not connecting to the Wi-Fi.**</span></span>

<span data-ttu-id="8d249-120">Der Status "Erfolgreich" bedeutet, dass Intune das Profil wie konfiguriert erfolgreich bereitgestellt hat.</span><span class="sxs-lookup"><span data-stu-id="8d249-120">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="8d249-121">Diese Konfigurationen entsprechen aber möglicherweise nicht Ihren Netzwerk- und/oder Authentifizierungsanforderungen.</span><span class="sxs-lookup"><span data-stu-id="8d249-121">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="8d249-122">Weitere Einzelheiten zu der versuchten Verbindung finden Sie in den Protokollen in der Infrastruktur und im Authentifizierungsdienst (auf dem WLAN-Zugriffspunktcontroller und dem NPS/Radius-Server).</span><span class="sxs-lookup"><span data-stu-id="8d249-122">For more details about the attempted connection, review logs in the infrastructure and authentication service (on the Wi-Fi Access point controller and NPS/Radius server).</span></span> <span data-ttu-id="8d249-123">Möglicherweise müssen Sie mit Ihrem Netzwerkinfrastrukturteam oder dem WLAN-Drittanbieterhersteller zusammenarbeiten, um Protokolle zu sammeln und zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="8d249-123">You might have to work with your network infrastructure team, or the third-party Wi-Fi vendor, to gather and review logs.</span></span>