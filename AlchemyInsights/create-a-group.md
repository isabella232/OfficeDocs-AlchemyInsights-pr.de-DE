---
title: Erstellen einer Gruppe
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816355"
---
# <a name="create-a-group"></a>Erstellen einer Gruppe

In diesem Thema wird die Gruppenerstellung beschrieben.

**Berechtigung zum Erstellen einer Gruppe**

Stellen Sie sicher, dass Sie autorisiert sind, eine neue Gruppe zu erstellen. Globale Administratoren können die Gruppenerstellung im Microsoft Azure-Portal oder im Access Panel deaktivieren. Möglicherweise benötigen Sie einen Administrator, um die neue Gruppe für Sie zu erstellen oder Ihnen die entsprechenden Berechtigungen zu erteilen.

**Verwalten von Gruppenerstellungsberechtigungen**

1. Globale Administratoren können Gruppenerstellungsberechtigungen (aus sicherheitsbezogenen Gründen) oder Office 365-Gruppen verwalten, die im Azure-Portal oder im Zugriffsbereich erstellt wurden, indem sie unter **Alle** Gruppen  >  **Allgemein (Einstellungen)** die Optionen "Benutzer können Sicherheitsgruppen in Azure-Portalen erstellen" oder "Benutzer können Office 365-Gruppen in Azure-Portalen erstellen" auswählen.
2. Sie können die Gruppenerstellung auch einschränken, um eine Gruppe von Benutzern auszuwählen, wenn Sie über eine Azure Active Directory P1 Premium-Lizenz verfügen.

**Deaktivieren der Willkommensbenachrichtigung für neue Office 365-Gruppenmitglieder**

Die Willkommensbenachrichtigung, die an Benutzer gesendet wird, die Office 365-Gruppen hinzugefügt werden, kann deaktiviert werden, indem **UnifiedGroupWelcomeMessageEnabled** in Powershell auf False gesetzt wird. Erfahren Sie [hier](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true) mehr über diese Einstellung.

