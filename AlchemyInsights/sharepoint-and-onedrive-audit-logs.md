---
title: Klassische SharePoint-Überwachungsprotokollberichte
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662207"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint-und OneDrive-Überwachungsprotokolle

## <a name="sharepoint-classic-audit-logs"></a>Klassische SharePoint-Überwachungsprotokolle

Die SPO-Legacy Überwachung wurde zu einem einheitlichen Überwachungsprotokoll migriert. Alle SPO-Legacy-Überwachungsberichte werden nun über unterstützt, und die Legacy-Überwachungssignale wurden zu "ausgehend" migriert.

Wichtige Änderungen:

* Trimmen ist nicht als Funktion verfügbar.
* Das Auswählen bestimmter zu überwachenden Ereignisse ist nicht verfügbar. In [diesem Dokument](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) finden Sie eine vollständige Liste überwachter Ereignisse, die standardmäßig verfügbar sind.
* Die Option **Speicherort** unter **angepasste Berichte** ist nicht verfügbar.
* Die Option zum **Öffnen oder Herunterladen von Dokument** Ereignissen ist nicht verfügbar.

[Konfigurieren von Überwachungseinstellungen für eine Websitesammlung](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>Moderne Unified Audit-Protokolle von SharePoint und OneDrive aus Compliance

* [Aktivieren/Deaktivieren der einheitlichen Überwachungsprotokollierung](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

In SharePoint oder OneDrive ist keine zusätzliche Konfiguration erforderlich.

Verwenden Sie die Überwachungs Protokollierungs Suche, um die Aktivität der Datei (en), des Ordners (s), des (der) Benutzers (s), der Berechtigungen zu überprüfen:

* [Datei- und Seitenaktivitäten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Ordneraktivitäten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Freigabe- und Zugriffsanforderungsaktivitäten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Synchronisierungsaktivitäten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Websiteverwaltungsaktivitäten](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Weitere Informationen zum Abrufen dieser Ereignisse finden Sie unter [Durchsuchen des Überwachungsprotokolls](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
