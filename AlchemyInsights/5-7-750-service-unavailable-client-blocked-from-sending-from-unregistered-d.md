---
title: 1048 5.7.750-Dienst ist nicht verfügbar. Vom Senden von nicht registrierten Domänen blockierter Client
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 8cf6d70b-9a78-4f04-ac59-7ffcf44ffd22
ms.custom: 1048
ms.openlocfilehash: 06be6babc524ae0d8065355218426c695f49be66
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31856619"
---
# <a name="57750-client-blocked-from-sending-from-unregistered-domain"></a>5.7.750-Client vom Senden von nicht registrierten Domäne blockiert

Der Fehler tritt auf, wenn eine größere Anzahl von Nachrichten von Domänen gesendet wird, die in Office 365 nicht bereitgestellt werden (als akzeptierte Domänen hinzugefügt und validiert).

Um diesen Fehler zu vermeiden, können Sie einen zertifikatbasierten Nachrichtenübermittlungs-Konnektor verwenden, in dem die Domäne des Zertifikats eine Bereitstellungsdomäne ist, oder Sie können alle sendenden Domänen einrichten.
