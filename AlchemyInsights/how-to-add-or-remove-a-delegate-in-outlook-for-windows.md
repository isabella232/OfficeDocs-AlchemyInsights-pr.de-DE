---
title: Vorgehensweise hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3800004"
- "7334"
ms.openlocfilehash: fcbd6082c104f0e1bca022a23cbbeb6e3363a6c5
ms.sourcegitcommit: c069f1b53567ad14711c423740f120439a312a60
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/04/2020
ms.locfileid: "49571836"
---
# <a name="how-to-add-or-remove-a-delegate-in-outlook-for-windows"></a>Vorgehensweise hinzufügen oder Entfernen einer Stellvertretung in Outlook für Windows

So fügen Sie in Outlook für Windows eine Stellvertretung hinzu: 

1. Klicken Sie auf die Registerkarte **Datei** , gefolgt von den **Kontoeinstellungen**, und wählen Sie dann **Stellvertretungszugriff** aus.
2. Klicken Sie auf **Hinzufügen**. Wenn **Add** nicht angezeigt wird, ist zwischen Outlook und Exchange möglicherweise keine aktive Verbindung vorhanden. In der Outlook-Statusleiste wird der Verbindungsstatus angezeigt.
3. Geben Sie den Namen der Person ein, die Sie als Stellvertreter festlegen möchten, oder suchen Sie den Namen in der Liste mit den Suchergebnissen aus, und wählen Sie ihn aus.

    > [!NOTE]
    > Bei der Stellvertretung muss es sich um eine Person in der globalen Exchange-Adressliste (GAL) Ihrer Organisation handeln.
4. Klicken Sie auf **Hinzufügen** , gefolgt von **OK**.
5. Übernehmen Sie im Dialogfeld **Berechtigungen delegieren** die Standard Berechtigungseinstellungen, oder wählen Sie benutzerdefinierte Zugriffsebenen für Exchange-Ordner aus.

    - Wenn ein Stellvertreter die Berechtigung zum Arbeiten nur mit Besprechungsanfragen und-Antworten benötigt, werden die Standard Berechtigungseinstellungen wie **Stellvertreter Kopien von Besprechungs bezogenen Nachrichten erhalten, die an mich gesendet** wurden, genügen. Sie können die Einstellung **Posteingangs** Berechtigung auf **None** belassen. Besprechungsanfragen und-Antworten gelangen direkt in den Posteingang des Stellvertreters.

    > [!NOTE]
    > Standardmäßig wird der Stellvertretung die Berechtigung **Editor (Elemente lesen, erstellen und ändern)** für den Ordner **Kalender** erteilt. Wenn der Stellvertreter auf eine Besprechung in Ihrem Namen antwortet, wird dieser automatisch Ihrem **Kalender** Ordner hinzugefügt.

5. Um eine Nachricht zu senden, um die Stellvertretung über die geänderten Berechtigungen zu benachrichtigen, aktivieren Sie das Kontrollkästchen **eine Nachricht wird automatisch an delegierende dieser Berechtigungen gesendet** .
6. Wenn Sie möchten, aktivieren Sie das Kontrollkästchen **Stellvertretung kann private Elemente anzeigen** .

    > [!IMPORTANT]
    > Diese Einstellung wirkt sich auf alle Exchange-Ordner aus. Dies umfasst alle Ordner "e-Mail", "Kontakte", "Kalender", "Aufgaben", "Notizen" und "Journal". Es gibt keine Möglichkeit, privaten Elementen nur in bestimmten Ordnern Zugriff zu gewähren.

7. Wählen Sie **OK** aus.

    > [!NOTE]
    >
    > - Nachrichten, die mit Berechtigungen zum Senden im Auftrag von gesendet werden, umfassen sowohl die Stellvertretung als auch ihre Namen neben **aus**. Wenn eine Nachricht mit "Senden als"-Berechtigungen gesendet wird, wird nur Ihr Name angezeigt.
    > - Nachdem Sie eine Person als Stellvertretung hinzugefügt haben, können Sie Ihr Exchange-Postfach Ihrem Outlook-Profil hinzufügen. Anweisungen finden Sie unter [Verwalten der e-Mails und Kalenderelemente einer anderen Person](https://support.microsoft.com/office/manage-another-person-s-mail-and-calendar-items-afb79d6b-2967-43b9-a944-a6b953190af5).

So entfernen Sie eine Stellvertretung in Outlook für Windows:

1. Klicken Sie auf die Registerkarte **Datei** .
2. Klicken Sie auf **Kontoeinstellungen** gefolgt von **Stellvertretungszugriff**.
3. Wählen Sie den Namen des Stellvertreters aus, für den Sie Berechtigungen ändern möchten, und klicken Sie dann auf **Entfernen** , gefolgt von **OK**.
