---
title: Probleme mit dem VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505209"
---
# <a name="vpn-related-issues"></a><span data-ttu-id="f9733-102">Probleme mit dem VPN</span><span class="sxs-lookup"><span data-stu-id="f9733-102">VPN related issues</span></span>

<span data-ttu-id="f9733-103">Die erfolgreiche Implementierung von VPN-Konnektivität für MDM-Clients hängt von einem bereitgestellten Profil ab, das die Anforderungen der VPN-Infrastruktur korrekt widerspiegelt.</span><span class="sxs-lookup"><span data-stu-id="f9733-103">Successful implementation of VPN connectivity for MDM clients depends on a deployed profile that correctly reflects the requirements of the VPN infrastructure.</span></span> <span data-ttu-id="f9733-104">Die entsprechenden Einstellungen für die von Ihnen untersuchten Clientplattformen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="f9733-104">For the appropriate settings for the client platforms you are investigating, see:</span></span> 

[<span data-ttu-id="f9733-105">Geräteeinstellungen für Windows 10 und Windows Holographic zum Hinzuzufügen von VPN-Verbindungen mithilfe von Intune</span><span class="sxs-lookup"><span data-stu-id="f9733-105">Windows 10 and Windows Holographic device settings to add VPN connections using Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[<span data-ttu-id="f9733-106">Hinzufügen von VPN-Einstellungen auf iOS- und iPadOS-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f9733-106">Add VPN settings on iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-ios)  
[<span data-ttu-id="f9733-107">Android-Geräteeinstellungen zur VPN-Konfiguration in Intune</span><span class="sxs-lookup"><span data-stu-id="f9733-107">Android device settings to configure VPN in Intune</span></span>](https://docs.microsoft.com/intune/vpn-settings-android)  
[<span data-ttu-id="f9733-108">Hinzufügen von VPN-Einstellungen macOS-Geräten in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f9733-108">Add VPN settings on macOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

<span data-ttu-id="f9733-109">Wenn Ihr VPN-Profil zertifikatsbasierte Authentifizierung verwendet, stellen Sie sicher, dass die mit dem VPN-Profil verknüpften Stammzertifikat- und Clientauthentifizierungszertifikat-Profile erfolgreich bereitgestellt werden.</span><span class="sxs-lookup"><span data-stu-id="f9733-109">If your VPN profile uses certificate based authentication, make sure that the root certificate and client authentication certificate profiles linked to the VPN profile are deployed successfully.</span></span>

<span data-ttu-id="f9733-110">**Häufig auftretende Probleme**</span><span class="sxs-lookup"><span data-stu-id="f9733-110">**Common Issues**</span></span>

<span data-ttu-id="f9733-111">**Ich habe ein VPN-Profil auf einem Gerät bereitgestellt. Intune zeigt an, dass dies erfolgreich war, aber das Gerät verbindet sich nicht mit dem VPN.**</span><span class="sxs-lookup"><span data-stu-id="f9733-111">**I deployed a VPN profile to a device. Intune is showing that it was successful, but the device is not connecting to the VPN.**</span></span>

<span data-ttu-id="f9733-112">Der Status "Erfolgreich" bedeutet, dass Intune das Profil wie konfiguriert erfolgreich bereitgestellt hat.</span><span class="sxs-lookup"><span data-stu-id="f9733-112">A successful status means that Intune has successfully deployed the profile as configured.</span></span> <span data-ttu-id="f9733-113">Diese Konfigurationen entsprechen aber möglicherweise nicht Ihren Netzwerk- und/oder Authentifizierungsanforderungen.</span><span class="sxs-lookup"><span data-stu-id="f9733-113">However, these configurations might not match your network and/or authentication requirements.</span></span> <span data-ttu-id="f9733-114">Überprüfen Sie die Protokolle in der Infrastruktur und im Authentifizierungsdienst (auf dem VPN-Server und dem NPS/Radius-Server), um weitere Einzelheiten über die versuchte Verbindung zu erfahren.</span><span class="sxs-lookup"><span data-stu-id="f9733-114">Review logs in the infrastructure and authentication service (on the VPN server and NPS/Radius server) for more details about the attempted connection.</span></span> <span data-ttu-id="f9733-115">Möglicherweise müssen Sie mit Ihrem Netzwerkinfrastruktur-Team oder dem VPN-Drittanbietern zusammenarbeiten, um Protokolle zu erfassen und zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="f9733-115">You might need to work with your network infrastructure team, or the third-party VPN vendor, to gather and review logs.</span></span>

<span data-ttu-id="f9733-116">**Wenn ich ein benutzerdefiniertes VPN für iOS konfiguriere, wird das Feature "Pro-App-VPN" nicht zur Verfügung gestellt.**</span><span class="sxs-lookup"><span data-stu-id="f9733-116">**When I configure a custom VPN for iOS, the per-app VPN feature isn't made available.**</span></span>

<span data-ttu-id="f9733-117">Pro-App-VPN für iOS-Geräte in Intune steht derzeit für eine bestimmte Liste von Anbietern und Partnern zur Verfügung, die vor der Konfiguration eines Pro-App-VPNs auch die Zertifikatvoraussetzungen erfüllen müssen.</span><span class="sxs-lookup"><span data-stu-id="f9733-117">Per-app VPN for iOS devices in Intune is currently available to a specific list of providers and partners, who must also meet the certificate prerequisites before configuring a per-app VPN.</span></span> <span data-ttu-id="f9733-118">Weitere Informationen finden Sie unter [Einrichten eines Pro-App-VPN für iOS/iPadOS-Geräte in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app) einrichten.</span><span class="sxs-lookup"><span data-stu-id="f9733-118">For more info, see [Set up per-app Virtual Private Network (VPN) for iOS/iPadOS devices in Intune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app).</span></span> 

<span data-ttu-id="f9733-119">Weitere Informationen zu allen VPN-Verbindungstypen in Intune finden Sie unter [Erstellen von VPN-Profilen zum Herstellen einer Verbindung mit VPN-Servern in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="f9733-119">For more info about all VPN connection types in Intune, see [Create VPN profiles to connect to VPN servers in Intune](https://docs.microsoft.com/intune/vpn-settings-configure).</span></span>  

<span data-ttu-id="f9733-120">**iOS On-Demand-VPN wird nicht ausgelöst, wenn auf eine konfigurierte Domäne zugegriffen wird**</span><span class="sxs-lookup"><span data-stu-id="f9733-120">**iOS On-Demand VPN is not triggering when a configured domain is accessed**</span></span>

<span data-ttu-id="f9733-121">Um die automatischen VPN-Einstellungen zu testen, legen Sie die folgenden Werte fest:</span><span class="sxs-lookup"><span data-stu-id="f9733-121">To test automatic VPN settings, set the following values:</span></span>

<span data-ttu-id="f9733-122">Ich möchte Folgendes tun: **Jeden Verbindungsversuch auswerten**</span><span class="sxs-lookup"><span data-stu-id="f9733-122">I want to do the following: **Evaluate each connection attempt**</span></span> 

<span data-ttu-id="f9733-123">Auswählen, ob eine Verbindung hergestellt werden soll: **Verbinden, falls erforderlich**</span><span class="sxs-lookup"><span data-stu-id="f9733-123">Choose whether to connect: **Connect if needed**</span></span>

<span data-ttu-id="f9733-124">Wenn Benutzer auf diese Domänen zugreifen: **Ziel** *Domänenname*</span><span class="sxs-lookup"><span data-stu-id="f9733-124">When users access these domains: **target** *domain name*</span></span>

<span data-ttu-id="f9733-125">Wenn die vorstehende Konfiguration nicht erfolgreich ist, fügen Sie das folgende Element hinzu:</span><span class="sxs-lookup"><span data-stu-id="f9733-125">If the above configuration is not successful, add the following element:</span></span>

<span data-ttu-id="f9733-126">Wenn diese URL nicht erreichbar ist, VPN-Verbindung erzwingen: **BADURL**</span><span class="sxs-lookup"><span data-stu-id="f9733-126">When this URL is unreachable, force connect the VPN: **BADURL**</span></span>