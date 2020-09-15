---
title: Deaktivieren externer Gruppen
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: f7a1bbda3a54d2662bdfe21cda961c32456edb82
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704127"
---
# <a name="how-to-disable-external-groups"></a>Deaktivieren externer Gruppen

"Jammern" externes Messaging wendet Exchange-Transport Regeln (ETRs) an, eine Gruppe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden. Um Benutzer daran zu hindern, externe Gruppen zu erstellen, müssen Sie eine Exchange-Transportregel (ETR) konfigurieren und dann jammern konfigurieren, damit die Exchange-Transportregel zum Blockieren von externem Messaging verwendet wird.
  
Nachdem Sie eine Regel in Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass Sie in "jammern" angewendet wird:
  
- Melden Sie sich bei jammern als überprüfter Administrator an, und wechseln Sie im **Admin Center**zu C- **Inhalts-und Sicherheits \> Sicherheitseinstellungen.**

- Wählen Sie unter **externes Messaging** **die Option Erzwingen der Exchange Online Exchange-Transport Regeln (ETRs) in jammern aus.**

- Wählen Sie **Speichern** aus.

Weitere Informationen finden Sie unter [Disable External Messaging in a jammern Network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).
  