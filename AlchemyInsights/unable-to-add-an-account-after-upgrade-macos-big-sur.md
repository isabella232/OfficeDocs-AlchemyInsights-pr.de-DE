---
title: Nach dem Upgrade auf macOS 11.6 Big Sur kann kein Konto hinzugefügt werden
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13840"
- "9008627"
ms.openlocfilehash: a8176de71a1f67004e790a3a98943402a240f656
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446729"
---
# <a name="unable-to-add-an-account-after-upgrading-to-macos-116-big-sur"></a>Nach dem Upgrade auf macOS 11.6 Big Sur kann kein Konto hinzugefügt werden

Nach dem Upgrade auf macOS 11.6 wird Ihr OneDrive für Geschäfts-, Schul- oder Ihr persönliches Konto möglicherweise nicht in Ihrer Kontenliste angezeigt, und Sie können sich möglicherweise nicht bei einem zweiten Konto in der App anmelden.

Dies ist ein neu auftretendes Problem im Zusammenhang mit dem MacOS 11.6 Upgrade. Bis das Problem behoben ist, können Sie über das Web oder Ihr mobiles Gerät auf Ihre OneDrive Inhalte zugreifen. Microsoft arbeitet mit Apple daran, OneDrive Funktionalität wiederherzustellen.

Sie können die fehlende OneDrive Instanz auch manuell mithilfe von Terminal starten. 

**Hinweis**: Diese Problemumgehung funktioniert nur, bis OneDrive neu gestartet wird (entweder durch einen Computerneustart oder ein OneDrive App-Update).

Wenn es sich bei der fehlenden Instanz um Ihr persönliches Konto handelt, öffnen Sie Terminal, und geben Sie Folgendes ein:

`open "/Applications/OneDrive.app" --new --args /client=Personal`

Wenn es sich bei der fehlenden Instanz um Ihr Geschäfts-, Schul- oder Unikonto handelt, öffnen Sie Terminal, und geben Sie Folgendes ein:

`open "/Applications/OneDrive.app" --new --args /client=Business1`

