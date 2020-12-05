---
title: Microsoft Edge-Support für Microsoft Defender Application Guard
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/05/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004024"
- "7090"
ms.openlocfilehash: 65cbc867ea7d1c73ca2906f51f72aa3376f31b5d
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49576549"
---
# <a name="microsoft-edges-support-for-microsoft-defender-application-guard"></a>Microsoft Edge-Support für Microsoft Defender Application Guard

Entwickelt für Windows 10 und Microsoft Edge verwendet Application Guard einen Ansatz zur Hardware Isolierung, mit dem ein Benutzer eine nicht vertrauenswürdige Website innerhalb eines isolierten Hyper-V-fähigen Containers navigieren kann, der vom Hostbetriebssystem getrennt ist.

Ein Unternehmensadministrator definiert eine Liste vertrauenswürdiger Websites, Cloud-Ressourcen und interner Netzwerke. Wenn ein Benutzer eine Website besucht, die nicht in der Liste enthalten ist, wird die Website von Microsoft Edge im Container geöffnet. Dies bedeutet, dass der Host-PC geschützt bleibt und der Angreifer nicht auf die Enterprise-Daten zugreift, wenn die Website als bösartig einstellt wird.

Die Installation von Erweiterungen im Container wird ab Microsoft Edge Version 81 unterstützt und kann über eine Richtlinie gesteuert werden. Die updateURL-Adresse, die in der ExtensionInstallForcelist-Richtlinie verwendet wird, sollte als neutrale Ressource in den vom Application Guard verwendeten Netzwerk Isolierungs Richtlinien hinzugefügt werden.

Weitere Informationen finden Sie unter [Microsoft Edge Support for Microsoft Defender Application Guard](https://go.microsoft.com/fwlink/?linkid=2134229).
