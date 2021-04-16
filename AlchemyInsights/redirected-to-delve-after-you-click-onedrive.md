---
title: OneDrive for Business Web OneDrive-Umleitungen zu Delve
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
- "1870"
- "900072"
ms.openlocfilehash: 96f23585f7cbce672842f6330ba79816f24dbc41
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51799988"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Umgeleitet zu Delve, nachdem Sie auf OneDrive geklickt haben

Weitere Informationen finden Sie im [ausführlichen Handbuch zur Problembehandlung.](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)

Um dieses Problem zu beheben, muss der Administrator Benutzern das Recht zum Erstellen ihrer Website "Meine Websites" erteilen. Dies liegt daran, dass die OneDrive for #A0 auf "Meine Websites" erstellt wird.

Führen Sie die folgenden Schritte aus, um dieses Recht zu gewähren:

1. Klicken Sie im SharePoint Admin Center auf **Benutzerprofile**.

2. Klicken Sie **im Abschnitt Personen** auf **Benutzerberechtigungen verwalten.**

3. Fügen Sie Benutzer hinzu, die Berechtigungen zum Erstellen ihrer Website "Meine Websites" benötigen. Standardmäßig ist diese Einstellung auf Jeder außer externen **Benutzern festgelegt.**

4. Nachdem Sie den Benutzer, die Benutzer oder die Gruppe hinzugefügt haben, stellen Sie sicher, dass der hinzugefügte Benutzer, benutzer oder die Gruppe ausgewählt ist, scrollen Sie zum Abschnitt Berechtigungen, und aktivieren Sie dann das Kontrollkästchen neben Persönliche Website erstellen (erforderlich für persönlichen **Speicher, Newsfeed** und gefolgten Inhalt). 

5. Klicken **Sie auf OK,** und navigieren Sie dann zur OneDrive-Seite, um die Website zu erstellen.
