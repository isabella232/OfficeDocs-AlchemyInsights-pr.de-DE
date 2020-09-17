---
title: Verwenden des Office-Bereitstellungstools
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "918"
- "2000022"
ms.assetid: 7ff7cc06-76d0-468f-bd66-3f2760750d04
ms.openlocfilehash: 9698aa12ad73a021a3cc12c8517c1712c48d8385
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794910"
---
# <a name="using-the-office-deployment-tool-odt"></a>Verwenden des Office-Bereitstellungstools (ODT)

Verwenden Sie das Office-Bereitstellungs Tool (ODT), um Office 365 Versionen von Office bereitzustellen. Das Office-Bereitstellungs Tool (setup.exe) wird über die Befehlszeile ausgeführt und verwendet eine Konfigurations-XML-Datei, um festzulegen, welche Einstellungen beim Bereitstellen von Office angewendet werden sollen.
  
1. Laden Sie die neueste Version des Office-Bereitstellungstools aus dem [Microsoft Download Center](https://go.microsoft.com/fwlink/p/?LinkID=626065)herunter.

2. Verwenden Sie das [Office-Anpassungs Tool (OAT)](https://config.office.com) , um Ihre Bereitstellungseinstellungen auszuwählen und die XML-Konfigurationsdatei zu erstellen. Exportieren Sie die Konfigurationsdatei, und platzieren Sie Sie lokal in demselben Ordner, in dem sich die setup.exe befindet.

    **Hinweis:** Probleme mit der Office-Installation treten häufig aufgrund falsch konfigurierter oder ungültige Konfigurationsdateien auf. Um solche Probleme zu vermeiden, sollten Sie das Office-Anpassungs Tool verwenden, um die Konfigurationsdatei zu erstellen. Sie können auch vorhandene Konfigurationsdateien in das Office-Anpassungs Tool importieren.

3. Wechseln Sie an einer Eingabeaufforderung mit erhöhten Rechten zu dem Speicherort, an dem sich setup.exe befindet, und führen Sie das Office-Bereitstellungs Tool im Downloadmodus aus, und geben Sie die soeben gespeicherte Konfigurationsdatei an. In diesem Beispiel wird die Konfigurationsdatei Configuration.xml benannt:

```setup.exe /download Configuration.xml```

4. führen Sie das Office-Bereitstellungs Tool im configure-Modus aus, und geben Sie die Konfigurationsdatei an.

```setup.exe /configure Configuration.xml```

**Hinweis:** Sie müssen diesen Schritt auf dem Clientcomputer ausführen, auf dem Sie Office installieren möchten, und Sie benötigen lokale Administratorberechtigungen auf diesem Computer.

Weitere Informationen zur Verwendung des Office-Bereitstellungstools für Ihre Microsoft 365-Apps für Enterprise-Bereitstellungsszenarien finden Sie unter [Übersicht über das Office-Bereitstellungstool](https://docs.microsoft.com/deployoffice/overview-office-deployment-tool). Weitere Informationen zur Verwendung des Office-Anpassungstools finden Sie unter [Übersicht über das Office-Anpassungstool](https://docs.microsoft.com/DeployOffice/overview-of-the-office-customization-tool-for-click-to-run).
