---
title: Problembehandlung bei der Bereitstellung von Clientauthentifizierungszertifikaten
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
- "1546"
- "9000076"
ms.openlocfilehash: 698329d7705af320c9f679b92532b58ac84e6624
ms.sourcegitcommit: e90b918f02102cd9764881c2d8c914567c6b070e
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509051"
---
# <a name="troubleshooting-client-authentication-certificate-deployment"></a><span data-ttu-id="c0cf4-102">Problembehandlung bei der Bereitstellung von Clientauthentifizierungszertifikaten</span><span class="sxs-lookup"><span data-stu-id="c0cf4-102">Troubleshooting Client Authentication certificate deployment</span></span>

<span data-ttu-id="c0cf4-103">Intune-Profile für NDES/SCEP- und PKCS/PFX-Clientzertifikate werden häufig in Verbindung mit anderen Profiltypen wie WLAN, VPN und E-Mail verwendet, um Benutzern die Authentifizierung bei Unternehmensressourcen zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-103">Intune NDES/SCEP and PKCS/PFX Client certificates profiles are commonly used in conjunction with other profiles types such as Wifi, VPN, and email to allow users to authenticate to corporate resources.</span></span> <span data-ttu-id="c0cf4-104">Wenn diese Profiltypen mit einem Clientzertifikatprofil verknüpft sind, sind sie von der erfolgreichen Bereitstellung dieses Profils abhängig.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-104">When those profile types are linked to a client certificate profile are dependant on the successful deployment of that profile.</span></span>

<span data-ttu-id="c0cf4-105">Das anfängliche Einrichten der Infrastruktur und die zugehörige Konfiguration des Clientzertifikatprofils erfordern häufig eine Problembehandlung.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-105">Initial infrastructure setup and associated configuration of the Client Certificate profile often require troubleshooting.</span></span> <span data-ttu-id="c0cf4-106">Eine schrittweise Anleitung für eine erfolgreiche Einrichten des NDES-Connectors sowie eine Anleitung zur Problembehandlung, um Probleme mit der Bereitstellung von Zertifikaten zu isolieren, finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="c0cf4-106">For a step-by-step guide to successful setup of the NDES connector and troubleshooting guidance to isolate issues with certificate deployment, see:</span></span> 

- [<span data-ttu-id="c0cf4-107">Konfigurieren der Infrastruktur, sodass SCEP mit Intune unterstützt wird</span><span class="sxs-lookup"><span data-stu-id="c0cf4-107">Configure infrastructure to support SCEP with Intune</span></span>](https://support.microsoft.com/help/4459540/troubleshoot-ndes-configuration-for-use-with-intune)
- [<span data-ttu-id="c0cf4-108">Übersicht für die Problembehandlung von SCEP-Zertifikatprofilen mit Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c0cf4-108">Overview for troubleshooting SCEP certificate profiles with Microsoft Intune</span></span>](https://support.microsoft.com/help/4457481/troubleshooting-scep-certificate-profile-deployment-in-intune)

<span data-ttu-id="c0cf4-109">Verwenden Sie die referenzierten PowerShell-Skripts, um Ihre Konfiguration zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-109">Use the referenced powershell scripts to help verify your configuration.</span></span> <span data-ttu-id="c0cf4-110">Weitere Informationen finden Sie unter [Skripts für die Überprüfung des Intune-Zertifikat-Connectors](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span><span class="sxs-lookup"><span data-stu-id="c0cf4-110">For more info, see [Intune Certificate connector verification scripts](https://github.com/microsoftgraph/powershell-intune-samples/tree/master/CertificationAuthority).</span></span>

  
<span data-ttu-id="c0cf4-111">**Sonstige häufig auftretende Probleme**</span><span class="sxs-lookup"><span data-stu-id="c0cf4-111">**Other common issues**</span></span>

<span data-ttu-id="c0cf4-112">**Beim Versuch, den Intune-Zertifikat-Connector auf dem NDES-Connectorserver zu installieren, wird die Meldung „Das Kennwort in der Zertifikatanforderung kann nicht überprüft werden. Möglicherweise wurde es bereits verwendet. Rufen Sie ein neues Kennwort ab, um es mit diese Anforderung zu übermitteln.“ angezeigt.**</span><span class="sxs-lookup"><span data-stu-id="c0cf4-112">**When I try to install the Intune certificate connector on the NDES connector server, I get the message, "The password in the certificate request cannot be verified. It may have been used already. Obtain a new password to submit with this request."**</span></span>  

<span data-ttu-id="c0cf4-113">Diese Meldung bedeutet, dass Sie die Installation des Zertifikat-Connectors als Administrator ausführen müssen.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-113">This message means that you need to run the certificate connector installation as an Administrator.</span></span>

<span data-ttu-id="c0cf4-114">In einigen Umgebungen müssen die Server, auf denen das Intune-Zertifikat ausgeführt wird, einen Proxyserver zum Herstellen einer Verbindung mit Intune verwenden, weshalb der Zertifikat-Connector ebenfalls einen Proxy verwenden muss.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-114">In some environments, the servers where the Intune Certificate runs must use a proxy server to connect to Intune, and so the Certificate Connector must use a proxy.</span></span> <span data-ttu-id="c0cf4-115">Unter bestimmten Umständen ignoriert der NDES-Connector die konfigurierten Proxyeinstellungen, und es kann notwendig sein, die Proxyeinstellungen während der Ausführung im Sicherheitskontext von „LocalSystem“ zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-115">In some circumstances, the NDES Connector ignores the configured proxy settings, and it might be necessary to configure the proxy settings while running in the security context of LocalSystem.</span></span> 
 
<span data-ttu-id="c0cf4-116">Die Lösung besteht darin, Internet Explorer als SYSTEM auszuführen und einen Proxy in IE zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-116">The solution is to run Internet Explorer as SYSTEM and configure a proxy in IE.</span></span> <span data-ttu-id="c0cf4-117">Nach einem Neustart des Intune-Connectordiensts stellt der NDES-Connector eine Verbindung mit Intune her.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-117">After a restart of the Intune Connector Service, the NDES Connector connects to Intune.</span></span>

<span data-ttu-id="c0cf4-118">**Benutzergeräte empfangen keine SCEP-Zertifikate mehr von NDES.**</span><span class="sxs-lookup"><span data-stu-id="c0cf4-118">**User devices are no longer receiving SCEP certificates from NDES.**</span></span>

<span data-ttu-id="c0cf4-119">Es ist möglich, dass das Clientauthentifizierungszertifikat, das für den NDES-Server ausgestellt und während der NDES-Connectorinstallation angegeben wurde, abgelaufen oder nicht vorhanden ist.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-119">It is possible that the Client Authentication certificate issued to the NDES server, and specified during the NDES connector installation, has expired or is missing.</span></span> <span data-ttu-id="c0cf4-120">Problemlösung:</span><span class="sxs-lookup"><span data-stu-id="c0cf4-120">To resolve:</span></span> 
 
1. <span data-ttu-id="c0cf4-121">Deinstallieren Sie den NDES-Connector.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-121">Uninstall the NDES connector.</span></span>  
2. <span data-ttu-id="c0cf4-122">Verwenden Sie diese Details, um ein neues Clientauthentifizierungs- oder Serverauthentifizierungszertifikat anzufordern:</span><span class="sxs-lookup"><span data-stu-id="c0cf4-122">Use these details to request a new client authentication or server authentication certificate:</span></span> 
 
    - <span data-ttu-id="c0cf4-123">Antragstellername: CN=externer FQDN</span><span class="sxs-lookup"><span data-stu-id="c0cf4-123">Subject name: CN=external fqdn</span></span>  
    - <span data-ttu-id="c0cf4-124">Alternativer Antragstellername (beide sind erforderlich): DNS=externer FQDN, DNS=interner FQDN</span><span class="sxs-lookup"><span data-stu-id="c0cf4-124">Subject alternative name (both are required): DNS=external fqdn, DNS=internal fqdn</span></span> 
 
3. <span data-ttu-id="c0cf4-125">Installieren Sie den NDES-Connector erneut mit dem neuen Zertifikat.</span><span class="sxs-lookup"><span data-stu-id="c0cf4-125">Reinstall the NDES connector with the new certificate.</span></span>