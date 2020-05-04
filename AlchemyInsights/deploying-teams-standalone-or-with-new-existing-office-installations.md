---
title: Bereitstellen von Teams als eigenständig oder mit neuen oder vorhandenen Office-Installationen
ms.author: danbrown
author: DHB-MSFT
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000660"
- "2509"
ms.openlocfilehash: ffa91eaf333792af149feda25f9a377ed591b597
ms.sourcegitcommit: 7e06d9ec1dd462cbd882f088c997d012a032f04d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 05/04/2020
ms.locfileid: "44010217"
---
# <a name="deploying-teams-as-standalone-or-with-new-or-existing-office-installations"></a>Bereitstellen von Teams als eigenständig oder mit neuen oder vorhandenen Office-Installationen

Microsoft Teams ist jetzt im Rahmen ***neuer Installationen*** von Microsoft 365 apps for Enterprise, Microsoft 365 apps for Business und Office für Mac enthalten. Weitere Informationen finden Sie unter [wann werden Microsoft Teams in neue Office-Installationen aufgenommen?](https://docs.microsoft.com/deployoffice/teams-install#when-will-microsoft-teams-start-being-included-with-new-installations-of-microsoft-365-apps)

Außerdem werden Microsoft Teams, beginnend mit der Version 1906 im monatlichen Kanal, zu vorhandenen Installationen von Microsoft 365 apps for Enterprise (und Microsoft 365 apps for Business) auf Geräten mit Windows ***hinzugefügt*** , wenn Sie die vorhandene Installation auf die neueste Version aktualisieren. Weitere Informationen finden Sie unter [Was ist mit vorhandenen Installationen von Office?](https://docs.microsoft.com/deployoffice/teams-install#what-about-existing-installations-of-microsoft-365-apps)

> [!NOTE]
> Wenn Sie nicht auf diesen Rollout Zeitplan warten möchten, können Sie Microsoft Teams als eigenständig für Ihre Benutzer bereitstellen, indem Sie  [diese Anweisungen befolgen](https://docs.microsoft.com/MicrosoftTeams/msi-deployment)oder Ihre Benutzer Teams für sich [https://teams.microsoft.com/downloads](https://teams.microsoft.com/downloads)selbst installieren lassen.

Wenn Ihre Organisation nicht bereit ist, Teams bereitzustellen, haben wir die Schritte, die Sie ausführen können, um Teams von [neuen](https://docs.microsoft.com/deployoffice/teams-install#how-to-exclude-microsoft-teams-from-new-installations-of-microsoft-365-apps) oder [vorhandenen](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-control-the-installation-of-microsoft-teams) Installationen von Office ***auszuschließen*** . Wenn Sie möchten, dass Teams installiert werden, Sie aber nicht möchten, dass Teams nach der Installation automatisch für den Benutzer gestartet werden, finden Sie unter [verhindern, dass Microsoft Teams automatisch nach der Installation](https://docs.microsoft.com/deployoffice/teams-install#use-group-policy-to-prevent-microsoft-teams-from-starting-automatically-after-installation)gestartet wird.

Informationen zum ***Deinstallieren von Teams*** von einem Gerät mit Windows finden Sie unter Deinstallieren von [Microsoft Teams](https://support.office.com/article/3b159754-3c26-4952-abe7-57d27f5f4c81). Informationen zum Bereinigen von Microsoft Teams von mehreren Zielcomputern oder Benutzern finden Sie unter Cleanup von [Microsoft Teams-Bereitstellung](https://docs.microsoft.com/microsoftteams/scripts/powershell-script-teams-deployment-clean-up).

Wenn Sie freigegebene Computer, Remote Desktop Dienste (RDS) oder virtuelle Desktopinfrastruktur (VDI) verwenden, finden Sie weitere Informationen unter [Shared Computer and VDI Environments with Microsoft Teams](https://docs.microsoft.com/deployoffice/teams-install#shared-computer-and-vdi-environments-with-microsoft-teams).

Wenn Sie Office für Mac verwenden, finden Sie weitere Informationen unter [Microsoft Teams-Installationen auf einem Mac](https://docs.microsoft.com/deployoffice/teams-install#microsoft-teams-installations-on-a-mac).

> [!NOTE]
> Nachdem Microsoft Teams installiert wurde, wird es automatisch etwa alle zwei Wochen mit neuen Features und Qualitäts Updates [aktualisiert](https://docs.microsoft.com/deployoffice/teams-install#feature-and-quality-updates-for-microsoft-teams) . 