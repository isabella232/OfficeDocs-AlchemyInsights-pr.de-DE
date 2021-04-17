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
# <a name="teams-admin-center"></a>Teams Admin Center

Erfahren Sie mehr über das Verwalten von Teams mit dem [Teams Admin Center](https://docs.microsoft.com/microsoftteams/manage-teams-skypeforbusiness-admin-center).

Wenn Sie nicht auf das Team Admin Center zugreifen können, überprüfen Sie die folgenden Punkte:

- Stellen Sie sicher, dass Sie die entsprechenden [Office 365-IP-Adressen und -URL](https://docs.microsoft.com/Office365/Enterprise/office-365-ip-web-service) in jedem Gerät des Umkreisnetzwerks (Firewall usw.) oder in den Firewallregeln auf dem lokalen Computer zugelassen haben.
- Vergewissern Sie sich, dass die Anmeldeinformationen, die Sie für den Zugriff auf das Teams Admin Portal verwenden, Ihrem Benutzernamen entspricht, der im [Microsoft 365-Verwaltungsportal](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) aufgelistet ist.

Wenn Benutzer nicht im Team Admin Center angezeigt werden, überprüfen Sie die folgenden Punkte:

- Haben Sie in den letzten 24 Stunden Benutzer erstellt oder Lizenzen zugewiesen? Stellen Sie sicher, dass Sie mindestens 24 Stunden warten, bevor Sie ein Supportticket öffnen.
- Überprüfen Sie, ob Sie geeignete Lizenzen zugewiesen haben.
- Wenn Sie über ein lokales Active Directory verfügen, stellen Sie sicher, dass [der Wert von „msRTCSIP-PrimaryUserAddress“ oder die SIP-Adresse im Feld „ProxyAddresses“ in Ihrem lokalen Active Directory eindeutig ist und das Format dem „](https://docs.microsoft.com/skypeforbusiness/troubleshoot/online-configuration/msrtcsip-primaryuseraddress-proxyaddaddress)sip:**Benutzernamen**“ des Benutzers aus dem [Microsoft 365 Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) entspricht.
- Wenn Sie beabsichtigen, eine Bereitstellung von Skype for Business Server beizubehalten, und Sie Benutzer sowohl lokal als auch in Online haben, befolgen Sie **„Einrichten von Hybrid mit Teams und Skype for Business Online“** in Ihrer Skype for Business Server-Systemsteuerung, und verschieben Sie die Benutzer nach Online.
