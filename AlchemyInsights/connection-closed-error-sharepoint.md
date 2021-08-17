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
ms.openlocfilehash: f0f82eaaa00d71992af445bb89346fb85bad3ade5d120b25ad3a6ea4f9674893
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/11/2021
ms.locfileid: "57883318"
---
# <a name="the-underlying-connection-was-closed-error-in-sharepoint"></a>Fehler "Die zugrunde liegende Verbindung wurde geschlossen" in SharePoint

Wenn in SharePoint die Fehlermeldung „Die zugrunde liegende Verbindung wurde geschlossen“ angezeigt wird, könnte dies mit dem Ende von TLS 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie in den folgenden Artikeln:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

Wenn Benutzer Windows 7 verwenden, sollten sie unbedingt [TLS-Verschlüsselungssammlungen in Windows 7](https://docs.microsoft.com/windows/win32/secauthn/tls-cipher-suites-in-windows-7) überprüfen.