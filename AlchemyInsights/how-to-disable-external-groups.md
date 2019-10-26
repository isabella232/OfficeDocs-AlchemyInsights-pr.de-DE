---
title: Deaktivieren externer Gruppen
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739492"
---
# <a name="how-to-disable-external-groups"></a>Deaktivieren externer Gruppen

"Jammern" externes Messaging wendet Exchange-Transport Regeln (ETRs) an, eine Gruppe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um Benutzer daran zu hindern, externe Gruppen zu erstellen, müssen Sie eine Exchange-Transportregel (ETR) konfigurieren und dann jammern konfigurieren, damit die Exchange-Transportregel zum Blockieren von externem Messaging verwendet wird.
  
Nachdem Sie eine Regel in Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass Sie in "jammern" angewendet wird:
  
- Melden Sie sich bei jammern als überprüfter Administrator an, und wechseln Sie im **Admin Center**zu C- **Inhalts \> -und Sicherheits Sicherheitseinstellungen.**

- Wählen Sie unter **externes Messaging** **die Option Erzwingen der Exchange Online Exchange-Transport Regeln (ETRs) in jammern aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter [Disable External Messaging in a jammern Network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  