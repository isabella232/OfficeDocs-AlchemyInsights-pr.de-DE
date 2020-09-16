---
title: Probleme mit dem VPN
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
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726090"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="b80c1-102">Probleme mit dem VPN</span><span class="sxs-lookup"><span data-stu-id="b80c1-102">VPN related issues</span></span>

<span data-ttu-id="b80c1-103">Die erfolgreiche Implementierung von VPN-Konnektivität für MDM-Clients hängt von einem bereitgestellten Profil ab, das die Anforderungen der VPN-Infrastruktur korrekt widerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="b80c1-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="b80c1-104">Die entsprechenden Einstellungen für die von Ihnen untersuchten Clientplattformen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="b80c1-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="b80c1-105">Geräteeinstellungen für Windows 10 und Windows Holographic zum Hinzuzufügen von VPN-Verbindungen mithilfe von Intune</span><span class="sxs-lookup"><span data-stu-id="b80c1-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="b80c1-106">Hinzufügen von VPN-Einstellungen auf iOS- und iPadOS-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b80c1-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="b80c1-107">Android-Geräteeinstellungen zur VPN-Konfiguration in Intune</span><span class="sxs-lookup"><span data-stu-id="b80c1-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="b80c1-108">Hinzufügen von VPN-Einstellungen macOS-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="b80c1-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="b80c1-109">Wenn Ihr VPN-Profil zertifikatsbasierte Authentifizierung verwendet, stellen Sie sicher, dass die mit dem VPN-Profil verknüpften Stammzertifikat- und Clientauthentifizierungszertifikat-Profile erfolgreich bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="b80c1-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="b80c1-110">**Häufig auftretende Probleme**</span><span class="sxs-lookup"><span data-stu-id="b80c1-110">**Common Issues**</span></span>

<span data-ttu-id="b80c1-111">**Ich habe ein VPN-Profil auf einem Gerät bereitgestellt. Intune zeigt an, dass dies erfolgreich war, aber das Gerät verbindet sich nicht mit dem VPN.**</span><span class="sxs-lookup"><span data-stu-id="b80c1-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="b80c1-112">Der Status "Erfolgreich" bedeutet, dass Intune das Profil wie konfiguriert erfolgreich bereitgestellt hat.</span><span class="sxs-lookup"><span data-stu-id="b80c1-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="b80c1-113">Diese Konfigurationen entsprechen aber möglicherweise nicht Ihren Netzwerk- und/oder Authentifizierungsanforderungen.</span><span class="sxs-lookup"><span data-stu-id="b80c1-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="b80c1-114">Überprüfen Sie die Protokolle in der Infrastruktur und im Authentifizierungsdienst (auf dem VPN-Server und dem NPS/Radius-Server), um weitere Einzelheiten über die versuchte Verbindung zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="b80c1-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="b80c1-115">Möglicherweise müssen Sie mit Ihrem Netzwerkinfrastruktur-Team oder dem VPN-Drittanbietern zusammenarbeiten, um Protokolle zu erfassen und zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="b80c1-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="b80c1-116">**Wenn ich ein benutzerdefiniertes VPN für iOS konfiguriere, wird das Feature "Pro-App-VPN" nicht zur Verfügung gestellt.**</span><span class="sxs-lookup"><span data-stu-id="b80c1-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="b80c1-117">Pro-App-VPN für iOS-Geräte in Intune steht derzeit für eine bestimmte Liste von Anbietern und Partnern zur Verfügung, die vor der Konfiguration eines Pro-App-VPNs auch die Zertifikatvoraussetzungen erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="b80c1-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="b80c1-118">Weitere Informationen finden Sie unter [Einrichten eines Pro-App-VPN für iOS/iPadOS-Geräte in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) einrichten.</span><span class="sxs-lookup"><span data-stu-id="b80c1-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="b80c1-119">Weitere Informationen zu allen VPN-Verbindungstypen in Intune finden Sie unter [Erstellen von VPN-Profilen zum Herstellen einer Verbindung mit VPN-Servern in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="b80c1-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="b80c1-120">**iOS On-Demand-VPN wird nicht ausgelöst, wenn auf eine konfigurierte Domäne zugegriffen wird**</span><span class="sxs-lookup"><span data-stu-id="b80c1-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="b80c1-121">Um die automatischen VPN-Einstellungen zu testen, legen Sie die folgenden Werte fest:</span><span class="sxs-lookup"><span data-stu-id="b80c1-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="b80c1-122">Ich möchte Folgendes tun: **Jeden Verbindungsversuch auswerten**</span><span class="sxs-lookup"><span data-stu-id="b80c1-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="b80c1-123">Auswählen, ob eine Verbindung hergestellt werden soll: **Verbinden, falls erforderlich**</span><span class="sxs-lookup"><span data-stu-id="b80c1-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="b80c1-124">Wenn Benutzer auf diese Domänen zugreifen: **Ziel** *Domänenname*</span><span class="sxs-lookup"><span data-stu-id="b80c1-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="b80c1-125">Wenn die vorstehende Konfiguration nicht erfolgreich ist, fügen Sie das folgende Element hinzu:</span><span class="sxs-lookup"><span data-stu-id="b80c1-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="b80c1-126">Wenn diese URL nicht erreichbar ist, VPN-Verbindung erzwingen: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="b80c1-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>