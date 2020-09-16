---
title: OneDrive für Unternehmen-OneDrive wird weitergeleitet, um zu vertiefen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: faa2cf25270a3b74a12aeb63d23ce98b51e13cb6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47776378"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>Umgeleitet zu vertiefen, nachdem Sie auf OneDrive

Weitere Informationen finden Sie in unserem detaillierten [Leitfaden zur Problembehandlung](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning).

Um dieses Problem zu beheben, muss der Administrator Benutzern das Recht zum Erstellen Ihrer Website "Meine Websites" erteilen. Dies liegt daran, dass die OneDrive für Unternehmen Seite auf "Meine Websites" erstellt wird.

Führen Sie die folgenden Schritte aus, um dieses Recht zu erteilen:

1. Klicken Sie im SharePoint Admin Center auf **Benutzerprofile**.

2. Klicken Sie im Abschnitt **Personen** auf **Benutzerberechtigungen verwalten**.

3. Hinzufügen von Benutzern, die Berechtigungen zum Erstellen Ihrer Website "Meine Websites" benötigen. Diese Einstellung ist standardmäßig auf **jeder außer auf externe Benutzer**festgelegt.

4. Nachdem Sie den Benutzer, die Benutzer oder die Gruppe hinzugefügt haben, stellen Sie sicher, dass der hinzugefügte Benutzer, die Benutzer oder die Gruppe ausgewählt ist, führen Sie einen Bildlauf zum Abschnitt **Berechtigungen** durch, und aktivieren Sie dann das Kontrollkästchen neben **persönliche Website erstellen (erforderlich für persönlichen Speicher, Newsfeed und gefolgter Inhalt)**.

5. Klicken Sie auf **OK**, und lassen Sie den Benutzer zur Seite OneDrive wechseln, um die Website zu erstellen.
