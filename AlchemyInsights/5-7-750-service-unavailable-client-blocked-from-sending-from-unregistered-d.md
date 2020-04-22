---
title: 1048 5.7.750-Dienst ist nicht verfügbar. Vom Senden von nicht registrierten Domänen blockierter Client
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom:
- "1048"
- "3100026"
ms.openlocfilehash: 48b9c2de27f8d7f52215c3a3d547bdf746a3a4cd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43676712"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750 Client darf keine Mails von unregistrierter Domäne senden

Der Fehler tritt auf, wenn eine große Anzahl von Nachrichten von Domänen gesendet werden, die nicht in Ihrem Mandanten bereitgestellt werden (als akzeptierte Domänen hinzugefügt und überprüft).

Um diesen Fehler zu vermeiden, können Sie einen zertifikatbasierten e-Mail-Fluss-Konnektor verwenden, bei dem es sich bei der Domäne des Zertifikats um eine Bereitstellungsdomäne handelt, oder Sie können alle sendenden Domänen zur Verfügung stellen.
