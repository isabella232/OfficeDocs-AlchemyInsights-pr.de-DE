---
title: Erstellen einer Gruppe
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 11/17/2020
ms.locfileid: "49086395"
---
# <a name="create-a-group"></a>Erstellen einer Gruppe

In diesem Thema wird die Gruppenerstellung beschrieben.

**Berechtigung zum Erstellen einer Gruppe**

Stellen Sie sicher, dass Sie berechtigt sind, eine neue Gruppe zu erstellen. Globale Administratoren können die Gruppenerstellung im Azure-Portal oder im Access-Bereich deaktivieren. Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen entsprechende Berechtigungen zu erteilen.

**Verwalten von Berechtigungen für die Gruppenerstellung**

1. Globale Administratoren können Berechtigungen zur Gruppenerstellung (aus Sicherheitsgründen) oder Office 365 Gruppen, die im Azure-Portal oder im Access-Panel erstellt wurden, verwalten, indem Sie "Benutzer können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365 Gruppen in Azure-Portalen erstellen" in **allen Gruppen**  >  **Allgemein (Einstellungen)** auswählen.
2. Sie können die Gruppenerstellung auch so einschränken, dass eine Gruppe von Benutzern ausgewählt wird, wenn Sie über eine Azure Active Directory P1 Premium-Lizenz verfügen.

**Deaktivieren der Willkommens Benachrichtigung für neue Office 365 Gruppenmitglieder**

Die Willkommens Benachrichtigung, die an Benutzer gesendet wird, die Office 365 Gruppen hinzugefügt werden, kann deaktiviert werden, indem in PowerShell **UnifiedGroupWelcomeMessageEnabled** auf false festgelegt wird. [Hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)erfahren Sie mehr über diese Einstellung.

