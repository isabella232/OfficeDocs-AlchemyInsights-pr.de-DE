---
title: Probleme mit dem Onboarding-Computern
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6023"
- "9002913"
ms.openlocfilehash: c3203ed68eb19d5f6d75eb2269094bb0422b14cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47676881"
---
# <a name="issues-with-onboarding-machines"></a>Probleme mit dem Onboarding-Computern

Möglicherweise haben Sie Probleme mit Onboarding-Computern beim MDATP-Dienst. Wenn Sie auf den Endbenutzercomputer zugreifen können, führen Sie die folgenden Schritte aus:

1. Laden Sie das [Clientverbindungsuntersuchung](https://aka.ms/mdatpanalyzer)-Diagnosetool herunter.
2. Extrahieren Sie MDATPAnalyzer.cmd, und führen Sie es aus.
3. Suchen Sie das Diagnoseprotokoll im Ordner „MDATPClientAnalyzerResult“, dem gleichen Ordner, in dem das Untersuchungstool heruntergeladen wird.
4. Überprüfen Sie die Protokolldatei „MDATPClientAnalyzer.txt“, um Probleme mit der Verbindung oder Internetproxyeinstellungen zu finden.