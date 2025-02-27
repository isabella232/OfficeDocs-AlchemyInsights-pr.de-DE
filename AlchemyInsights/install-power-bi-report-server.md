---
title: Installieren Power BI-Berichtsserver
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1304"
- "2500001"
ms.openlocfilehash: 01cc2efc2dacc2fdf0b7b7f036bc18e1c75fd515348b72d5c4dde96949a51a2d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028579"
---
# <a name="install-power-bi-report-server"></a>Installieren Power BI-Berichtsserver

1. Suchen Sie den Speicherort der PowerBIReportServer.exe, und starten Sie das Installationsprogramm.

2. Wählen Sie **Power BI-Berichtsserver installieren** aus.

3. Wählen Sie eine zu installierende Edition aus, und wählen Sie dann **"Weiter"** aus.

4. Sie können in der Dropdownliste entweder "Evaluierung" oder "Entwicklerversion" auswählen.  Andernfalls können Sie einen Product Key für den Server eingeben, den Sie entweder vom Power BI-Dienst oder vom Volume License Service Center erworben haben. Weitere Informationen zum Abrufen Ihres Product Keys finden Sie im Abschnitt "Bevor Sie beginnen". Lesen Sie die Lizenzbedingungen, stimmen Sie diesen zu, und wählen Sie dann **"Weiter"** aus.

5. Sie müssen über eine Datenbank-Engine verfügen, um die Berichtsserverdatenbank zu speichern. Wählen Sie **"Weiter"** aus, um nur den Berichtsserver zu installieren.

6. Geben Sie den Installationsspeicherort für den Berichtsserver an. Wählen Sie **"Installieren"** aus, um fortzufahren.

7. Wählen Sie nach einer erfolgreichen Einrichtung **"Berichtsserver konfigurieren"** aus, um den Reporting Services Configuration Manager zu starten.

Sie benötigen keinen SQL Server Datenbank-Engine Server, der zum Zeitpunkt der Installation verfügbar ist. Sie benötigen eine, um Reporting Services nach der Installation zu konfigurieren.

Weitere Informationen: https://docs.microsoft.com/power-bi/report-server/install-report-server
