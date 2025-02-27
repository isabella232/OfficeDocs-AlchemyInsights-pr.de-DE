---
title: Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden
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
- "9002947"
- "5642"
ms.openlocfilehash: 7e667e22cd81f38a1a2c1385bf42e5227cb641480f4b505110ee7349a13f13a1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088395"
---
# <a name="hide-or-un-hide-office-365-groups-or-teams-from-address-list"></a>Office 365-Gruppen oder -Teams auf der Adressliste aus- oder einblenden

Verwenden Sie den folgenden EXO PowerShell-Befehl, um Office 365-Gruppen/-Teams auf Adresslisten (Globale Adressliste, GAL) von Exchange-Clients (Outlook, OWA) aus- oder einzublenden:

`
    Set-UnifiedGroup -Identity GroupName -HiddenFromAddressListsEnabled:<$true> or <$false>
`

Verwenden Sie den folgenden EXO PowerShell-Befehl, um die Office 365-Gruppen/-Teams von Exchange-Clients (Outlook, OWA) aus oder einzublenden:

`
    Set-unifiedGroup -Identity GroupName -HiddenFromExchangeClientsEnabled:<$true> or <$false>
`

- Detaillierte Anweisungen finden Sie unter [Ausblenden von Office 365-Gruppen auf der GAL und Exchange-Clients](https://docs.microsoft.com/schooldatasync/hide-office-365-groups-from-the-gal).
