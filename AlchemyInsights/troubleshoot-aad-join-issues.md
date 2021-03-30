---
title: Behandeln von Problemen mit der Azure AD-Verknüpfung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403873"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Behandeln von Problemen mit der Azure AD-Verknüpfung

1. Wenn Sie geräteregistrierungen zum ersten Mal einrichten, stellen Sie sicher, dass Sie die Einführung in die Geräteverwaltung [in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) überprüft haben, die Sie bei der Bereitstellung von Geräten in Azure AD unterstützt. 
1. Wenn Sie Geräte direkt bei Azure AD registrieren und sie bei Intune registrieren, müssen Sie [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) sicherstellen, dass Sie [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) konfiguriert haben und zuerst die Lizenzierung haben.
1. Stellen Sie sicher, dass Sie autorisiert sind, Vorgänge in Azure AD durchzuführen. Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.
1. Informationen zur Azure AD-Beitrittsimplementierung finden Sie unter [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).

Weitere Informationen zum Beheben gängiger Probleme bei der Azure AD-Teilnahme finden Sie unter Häufig gestellte Fragen zur [Azure Ad-Teilnahme](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) und für Windows 10 Pro-Geräte unter Nicht in der Lage, [Windows 10 Pro-Computer](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) zu Azure AD zu verbinden – Müssen auf aktualisieren – Microsoft Community
