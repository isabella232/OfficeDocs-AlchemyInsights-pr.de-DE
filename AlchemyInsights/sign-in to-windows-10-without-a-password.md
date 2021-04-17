---
title: Anmelden bei Windows 10 ohne Kennwort
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
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830545"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>Anmelden bei Windows 10 ohne Kennwort

Um zu vermeiden, dass Sie beim Starten von Windows ein Kennwort eingeben müssen, empfehlen wir, eine der sicheren Anmeldeoptionen für Windows Hello zu verwenden, z. B. eine PIN, Gesichtserkennung oder Fingerabdruck, sofern verfügbar. Wenn Sie die sichere Anmeldung wirklich deaktivieren möchten, lesen Sie die Anweisungen "Automatische Anmeldung bei Windows 10" weiter unten.

**Sichern von Windows Hello-Alternativen zum Kontokennwort**

Wechseln Sie **zu Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)). Verfügbare Anmeldeoptionen werden aufgelistet. Zum Beispiel:

![Anmeldeoptionen.](media/sign-in-options.png)

Klicken oder tippen Sie auf eine der Optionen, um sie zu konfigurieren. Wenn Sie Windows das nächste Mal starten oder entsperren, können Sie die neue Option anstelle eines Kennworts verwenden. 

**Automatische Anmeldung bei Windows 10**

**Hinweis:** Die automatische Anmeldung ist praktisch, führt jedoch zu einem Sicherheitsrisiko, insbesondere wenn auf Ihren PC mehrere Personen zugriffen können. 

1. Klicken oder tippen Sie **auf die Schaltfläche Start** in der Taskleiste.

2. Geben **Sie netplwiz ein,** und drücken Sie die EINGABETASTE, um das Fenster Benutzerkonten zu öffnen.

3. Klicken **Sie unter Benutzerkonten** auf das Konto, bei dem Sie sich automatisch anmelden möchten, wenn Windows gestartet wird.

4. Deaktivieren Sie das Kontrollkästchen "Benutzer müssen einen Benutzernamen und ein Kennwort eingeben, um diesen Computer zu verwenden".

    ![Benutzer müssen eine Benutzername- und Kennwortoption eingeben.](media/users-must-enter-username.png)

5. Klicken Sie auf **OK**. Sie werden aufgefordert, das Kennwort für das ausgewählte Konto einzugeben und zu bestätigen. Klicken Sie zum Abschließen auf **OK**. Wenn Windows 10 das nächste Mal gestartet wird, wird es sich automatisch bei dem ausgewählten Konto anmelden.
