---
title: Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 743b5917c08b0a49a8c5791bdeb59a1672dd0fc7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757299"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a>Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune

Die Möglichkeit, die Aktivierungssperre auf iOS-Geräten zu umgehen, erleichtert die Wiederherstellung in dem Szenario, in dem ein Benutzer die Aktivierungssperre auf einem Unternehmensgerät aktiviert und das Unternehmen verlässt.

Zu den Voraussetzungen für die Umgehung einer Aktivierungssperre gehören:

- Das Gerät wird "beaufsichtigt".
- Die Aktivierungssperre wird mithilfe der iOS-Geräteeinschränkungsrichtlinie in Intune erfolgreich aktiviert.

Außerdem sollten Sie beim Umgehen einer Aktivierungssperre:

- das zurückzusetzende Gerät physisch besitzen.
- vor dem Auslösen des Zurücksetzens den Code kopieren.

**Hinweis:** Beim Zurücksetzungscode wird nicht nach Groß-/Kleinschreibung unterschieden, sodass die Zeichen "-"-Zeichen nicht erforderlich sind.

Weitere Informationen finden Sie unter [Umgehen der Aktivierungssperre für überwachte iOS-Geräte mit Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).

**Häufig gestellte Fragen**

F: **Ich habe eine Remoteaktion zum Entfernen von Unternehmensdaten von einem Gerät gesendet, und jetzt ist das Gerät im Zustand „Ausstehend“ hängen geblieben.**

A: Damit eine Remoteaktion erfolgreich abgeschlossen werden kann, muss das Zielgerät online und fehlerfrei sein. In den folgenden Situationen bleibt die Remoteaktion 30 Tage lang im Zustand „Ausstehend“ oder bis das Gerät den Befehl bestätigt, falls Folgendes für das Gerät zutrifft:

- Das Gerät hat keine Verbindung.
- Das Gerät verliert seinen Verwaltungsstatus bei Intune.

Wenn Sie der Meinung sind, dass das Gerät keinen Check-In mehr vornimmt und dass es keine Unternehmensdaten entfernt, wählen Sie „Löschen“ aus. Durch das Löschen wird der Gerätedatensatz entfernt, sodass er nicht mehr in der Liste der Geräte in Intune angezeigt wird. Damit das Gerät wieder aktiv wird, muss der Benutzer das Gerät erneut registrieren.

F: **Warum sind bestimmte Remoteaktionen für mich nicht verfügbar?**

A: Nicht alle Plattformen unterstützen alle Remoteaktionen für Geräte. Die folgenden Remoteaktionen sind plattformspezifisch.

- Aktivierungssperre umgehen (nur iOS)
- Sauberer Start (nur Windows)
- Modus für verlorene Geräte (nur iOS)
- Gerät suchen (nur iOS)
- Neustart (nur Windows)

Weitere Details zu den einzelnen Aktionen finden Sie unter [Verfügbare Geräteaktionen](https://docs.microsoft.com/intune/device-management#available-device-actions).