---
title: Teams Admin Center
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
- "9002890"
- "5542"
ms.openlocfilehash: 4a3a0796cedd81919066d870c5ca99fe2e978cf8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826378"
---
# <a name="teams-admin-center"></a><span data-ttu-id="615aa-102">Teams Admin Center</span><span class="sxs-lookup"><span data-stu-id="615aa-102">Teams Admin Center</span></span>

<span data-ttu-id="615aa-103">Erfahren Sie mehr über das Verwalten von Teams mit dem [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span><span class="sxs-lookup"><span data-stu-id="615aa-103">Learn about managing Teams with the [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).</span></span>

<span data-ttu-id="615aa-104">Wenn Sie nicht auf das Team Admin Center zugreifen können, überprüfen Sie die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="615aa-104">If you are unable to access the Teams Admin Center, please check the following items:</span></span>

- <span data-ttu-id="615aa-105">Stellen Sie sicher, dass Sie die entsprechenden [Office 365-IP-Adressen und -URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) in jedem Gerät des Umkreisnetzwerks (Firewall usw.) oder in den Firewallregeln auf dem lokalen Computer zugelassen haben.</span><span class="sxs-lookup"><span data-stu-id="615aa-105">Verify that you have allowed the appropriate [Office 365 IP addresses and URL's](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) on any perimeter devices (firewall, etc.) or in the firewall rules on your local machine.</span></span>
- <span data-ttu-id="615aa-106">Vergewissern Sie sich, dass die Anmeldeinformationen, die Sie für den Zugriff auf das Teams Admin Portal verwenden, Ihrem Benutzernamen entspricht, der im [Microsoft 365-Verwaltungsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) aufgelistet ist.</span><span class="sxs-lookup"><span data-stu-id="615aa-106">Verify that the login you are using to access the Teams Admin Portal matches your username listed in the [Microsoft 365 Admin portal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>

<span data-ttu-id="615aa-107">Wenn Benutzer nicht im Team Admin Center angezeigt werden, überprüfen Sie die folgenden Punkte:</span><span class="sxs-lookup"><span data-stu-id="615aa-107">If users are not appearing in the Teams Admin Center, please check the following:</span></span>

- <span data-ttu-id="615aa-108">Haben Sie in den letzten 24 Stunden Benutzer erstellt oder Lizenzen zugewiesen?</span><span class="sxs-lookup"><span data-stu-id="615aa-108">Have you created users or assigned licenses in the last 24 hours?</span></span> <span data-ttu-id="615aa-109">Stellen Sie sicher, dass Sie mindestens 24 Stunden warten, bevor Sie ein Supportticket öffnen.</span><span class="sxs-lookup"><span data-stu-id="615aa-109">Please make sure you wait at least 24 hours before opening a support ticket.</span></span>
- <span data-ttu-id="615aa-110">Überprüfen Sie, ob Sie geeignete Lizenzen zugewiesen haben.</span><span class="sxs-lookup"><span data-stu-id="615aa-110">Verify you have assigned appropriate licenses?</span></span>
- <span data-ttu-id="615aa-111">Wenn Sie über ein lokales Active Directory verfügen, stellen Sie sicher, dass [der Wert von „msRTCSIP-PrimaryUserAddress“ oder die SIP-Adresse im Feld „ProxyAddresses“ in Ihrem lokalen Active Directory eindeutig ist und das Format dem „](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)sip:**Benutzernamen**“ des Benutzers aus dem [Microsoft 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) entspricht.</span><span class="sxs-lookup"><span data-stu-id="615aa-111">If you have an on-premise Active Directory, verify that [the value of msRTCSIP-PrimaryUserAddress or the SIP address in the ProxyAddresses field in your local Active Directory is unique and the format matches](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress) sip:**Username** of the user from the [Microsoft 365 admin center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users).</span></span>
- <span data-ttu-id="615aa-112">Wenn Sie beabsichtigen, eine Bereitstellung von Skype for Business Server beizubehalten, und Sie Benutzer sowohl lokal als auch in Online haben, befolgen Sie **„Einrichten von Hybrid mit Teams und Skype for Business Online“** in Ihrer Skype for Business Server-Systemsteuerung, und verschieben Sie die Benutzer nach Online.</span><span class="sxs-lookup"><span data-stu-id="615aa-112">If you intend to keep a Skype for Business Server deployment and have users homed on-premises and Online: follow the **"Set up hybrid with Teams and Skype for Business Online"** in your Skype for Business Server Control Panel and move users Online.</span></span>
