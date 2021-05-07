---
title: Der Fehler „Die zugrunde liegende Verbindung wurde geschlossen“ in SharePoint
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 04/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10802"
- "9006390"
ms.openlocfilehash: b64215b5b83ef1092eb58791e6dbb015b72d422d
ms.sourcegitcommit: 6c6b0c3885f33b08db929fe0b6496508d31fa2d6
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/06/2021
ms.locfileid: "52233425"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Fehler "Die zugrunde liegende Verbindung wurde geschlossen" in SharePoint

Wenn in SharePoint die Fehlermeldung „Die zugrunde liegende Verbindung wurde geschlossen“ angezeigt wird, könnte dies mit dem Ende von TLS 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie in den folgenden Artikeln:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.