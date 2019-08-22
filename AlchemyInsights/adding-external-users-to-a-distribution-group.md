---
title: Hinzufügen externer Benutzer zu einer Verteilergruppe
ms.author: v-crytho
author: CrystalThomasMS
ms.date: 8/22/2017
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: ce0c589e1661fb4607452fe2e8f897758b2718e8
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36494526"
---
# <a name="add-external-users-to-a-distribution-group"></a>Externe Benutzer zu einer Verteilergruppe hinzufügen?

Das Hinzufügen eines externen Kontakts zu einer Verteilergruppe (DG) erfolgt in einem zweistufigen Prozess:
  
1. Erstellen Sie einen e-Mail-Kontakt für den externen Benutzer:
    
    1. Wechseln Sie im Admin Center zur Seite **Benutzer** > [Kontakte](https://admin.microsoft.com/adminportal/home#/Contact) . 
    
    2. Wählen Sie **Kontakt hinzufügen**aus.
    
    3. Geben Sie die Informationen für Ihren Kontakt ein, und wählen Sie **Hinzufügen**aus.
    
2. Fügen Sie den e-Mail-Kontakt zu Ihrer GD hinzu:
    
    1. Wechseln Sie im Admin Center zur Seite **Gruppen** > [](https://admin.microsoft.com/adminportal/home#/groups) Gruppen. 
    
    2. Suchen Sie die GD, der Sie den externen Benutzer hinzufügen möchten, und wählen Sie Sie aus, um das Dialogfeld bearbeiten zu öffnen.
    
    3. Wählen Sie auf der Registerkarte **Mitglieder** die Option **Alle anzeigen und Mitglieder verwalten**aus. 
    
    4. Wählen Sie **Mitglieder hinzufügen**aus.
    
    5. Wählen Sie den e-Mail-Kontakt aus, den Sie im vorherigen Schritt erstellt haben, und wählen Sie dann **Speichern**aus.
    
Wenn Ihre externen Benutzer nach diesen Schritten keine e-Mails an die DG senden können oder keine e-Mails davon erhalten, kann es sein, dass die DG so gekennzeichnet ist, dass Sie nur e-Mails von internen Benutzern zulässt. Sie können diese Konfiguration überprüfen und nach den Anweisungen [hier](https://support.office.com/article/Fix-email-delivery-issues-for-error-code-5-7-133-in-Office-365-991abc19-7756-438f-abcb-39f69b80f284.aspx)korrigieren.
  
 **Hinweis:** Diese Anweisungen gelten nicht, wenn der Typ der Gruppe "Office 365 Gruppe" anstelle von "Verteilergruppe" lautet. Wenn dies der Fall ist, können Sie den externen Benutzer direkt aus Outlook zur Gruppe hinzufügen. Ausführliche Informationen zu Office 365 Gruppen sowie Anweisungen zum Hinzufügen externer Gäste finden Sie in [diesem Artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).
  