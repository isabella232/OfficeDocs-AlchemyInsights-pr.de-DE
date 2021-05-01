---
title: Probleme mit SharePoint auf Windows 7-Rechnern
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
- "9006484"
- "11070"
ms.openlocfilehash: 787f0e713cc95b590bc494868d5098a25131ac56
ms.sourcegitcommit: d33ab8c73d8af51da782094fb8f8abf7626f4df3
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/28/2021
ms.locfileid: "52066998"
---
# <a name="issues-with-sharepoint-on-windows-7-machines"></a>Probleme mit SharePoint auf Windows 7-Rechnern

Wenn Sie auf Windows 7-Rechnern bei der Arbeit mit SharePoint oder OneDrive Fehler erhalten, können diese mit der Veraltung von TLS 1.0/1.1 zusammenhängen. Weitere Informationen finden Sie unter:

- [Vorbereiten von TLS 1.2 in Office 365 und Office 365 GCC](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365)

- Windows 7 SP1/Windows 8 Clients müssen TLS1.2 aktiviert haben. Weitere Informationen unter [Authentifizierungsfehler treten auf, wenn der Client keine TLS 1.2-Unterstützung hat](https://review.docs.microsoft.com/sharepoint/troubleshoot/administration/authentication-errors-tls12-support)

- Installieren Sie KB3140245 und erstellen Sie den Registry-Wert. Weitere Informationen finden Sie unter  [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)

- Windows 7 SP1/Windows 8-Clients müssen sicherstellen, dass die neuesten TLS-Cipher-Suites installiert sind. Weitere Informationen unter [Microsoft Security Advisory 3042058](https://docs.microsoft.com/security-updates/SecurityAdvisories/2015/3042058). 


