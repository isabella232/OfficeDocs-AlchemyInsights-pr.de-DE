---
title: Dateien bei Bedarf
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: 846cda97ccd52fcb43ae4a44f73deeaaa6dc093d
ms.sourcegitcommit: b7bbe4c5419668ce8e84196db382032ca09cd176
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/08/2020
ms.locfileid: "47406572"
---
# <a name="configure-files-on-demand"></a>OneDrive-Dateien bei Bedarf konfigurieren

Mit OneDrive-Dateien bei Bedarf können Sie auf alle Ihre Dateien in OneDrive zugreifen, ohne alle herunterladen und Speicherplatz auf Ihrem Gerät nutzen zu müssen.

So konfigurieren Sie die Dateien bei Bedarf auf Ihrem PC:

1. Wählen Sie das weiße oder blaue **OneDrive** Cloudsymbol im Benachrichtigungsbereich der Windows-Taskleiste aus. Wählen Sie **Hilfe & Einstellungen** Zahnradsymbol > **Einstellungen**.
2. Aktivieren Sie auf der Registerkarte **Einstellungen** das Kontrollkästchen **Platz sparen und Dateien erst bei Verwendung herunterladen**.  

Sie können Dateien bei Bedarf auch mithilfe der Registrierung konfigurieren.

Wenn Sie diese Einstellung deaktivieren, weisen Windows 10-Benutzer das gleiche Synchronisierungsverhalten wie Benutzer der früheren Versionen von Windows auf, und sie können "Dateien bei Bedarf" nicht aktivieren. Wenn Sie diese Einstellung nicht konfigurieren, können die Benutzer „Dateien bei Bedarf“ aktivieren oder deaktivieren.

Durch Aktivieren dieser Richtlinie wird der folgende Registrierungsschlüsselwert auf 1 festgelegt. Das Deaktivieren dieser Richtlinie setzt den folgenden Registrierungsschlüsselwert auf 0.

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

Wenn die Dateien bei Bedarf-Option in „Einstellungen“ nicht angezeigt wird, stellen Sie sicher, dass der Starttyp des Dienstes „Windows-Clouddateien-Filter-Treiber“ auf 2 (AUTO_START) festgelegt ist. Das Aktivieren dieses Features setzt den folgende Registrierungsschlüsselwert auf 2.

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`