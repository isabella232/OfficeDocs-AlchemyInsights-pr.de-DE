---
title: Verwenden von Microsoft InTune-Sicherheitsbasislinien zum Konfigurieren von Windows 10-Geräten
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004135"
- "7211"
ms.openlocfilehash: 24257f1ac5752df1598d08fcfdb95ee2642adfea
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571828"
---
# <a name="use-microsoft-intune-security-baselines-to-configure-windows-10-devices"></a>Verwenden von Microsoft InTune-Sicherheitsbasislinien zum Konfigurieren von Windows 10-Geräten

InTune-Sicherheitsbasislinien tragen zum Schutz von Benutzern und Geräten bei. Sicherheitsbasislinien sind vorkonfigurierte Gruppen von Windows-Einstellungen, die verwendet werden, um eine bekannte Gruppe von Einstellungen und Standardwerten anzuwenden, die von den entsprechenden Sicherheitsteams empfohlen werden. Durch das Erstellen eines Sicherheitsbasis Profils in InTune erstellen Sie eine Vorlage, die aus mehreren Geräte Konfigurationsprofilen besteht.

Wenn Sie Sicherheitsbasislinien in Gruppen von Benutzern oder Geräten bereitstellen, werden die Einstellungen auf Geräte angewendet, die unter Windows 10 oder höher ausgeführt werden. Beispielsweise aktiviert die MDM-Sicherheitsbasislinie automatisch (1) BitLocker für Wechseldatenträger, (2) erfordert das Kennwort für das Entsperren eines Geräts, und (3) deaktiviert die Standardauthentifizierung. Wenn ein Standardwert für Ihre Umgebung nicht funktioniert, passen Sie die Basislinie an, um die erforderlichen Einstellungen anzuwenden.

Sicherheitsbasislinien helfen außerdem bei der Einrichtung eines End-to-End-sicheren Workflows in Microsoft 365. Im folgenden finden Sie einige Vorteile:

- Eine Sicherheitsbasislinie enthält die bewährten Methoden und Empfehlungen für Einstellungen, die sich auf die Sicherheit auswirken. Da InTune mit dem Windows-Sicherheitsteam arbeitet, das Basispläne für Gruppenrichtlinien erstellt, basieren diese Empfehlungen auf fundierten Anleitungen und umfangreichen Erfahrungen.
- Wenn Sie neu in InTune sind und sich nicht sicher sind, wo Sie beginnen sollen, können Sicherheitsbasislinien Ihnen helfen, ein sicheres Profil schnell zu erstellen und bereitzustellen.
- Wenn Sie derzeit eine Gruppenrichtlinie verwenden, ist die Migration zu InTune für Verwaltungszwecke mit Sicherheitsbasislinien wesentlich einfacher, da Sie in InTune integriert sind und innovative Funktionen für die Verwaltung umfassen.

Weitere Informationen finden Sie unter [Windows-Sicherheitsbasislinien](https://go.microsoft.com/fwlink/?linkid=2141503) und [Verwaltung mobiler Geräte](https://go.microsoft.com/fwlink/?linkid=2141701).