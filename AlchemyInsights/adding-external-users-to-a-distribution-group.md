---
title: Hinzufügen externer Benutzer zu einer Verteilergruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: d8c06c81ecc66df0fbaa4cac9908178cdc1d9c6bdc38d19010c7b55e9bca8776
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934832"
---
# <a name="add-external-users-to-a-distribution-group"></a>Hinzufügen externer Benutzer zu einer Verteilergruppe

Das Hinzufügen eines externen Kontakts zu einer Verteilergruppe (DG) besteht aus zwei Schritten:
  
1. Erstellen Eines E-Mail-Kontakts für den externen Benutzer:
    
    1. Wechseln Sie im Admin Center zur Seite  >  ["Kontakte](https://admin.microsoft.com/adminportal/home#/Contact) der Benutzer". 
    
    2. Wählen Sie **"Kontakt hinzufügen"** aus.
    
    3. Geben Sie die Informationen für Ihren Kontakt ein, und wählen Sie **"Hinzufügen"** aus.
    
2. Fügen Sie den E-Mail-Kontakt zu Ihrer DG hinzu:
    
    1. Wechseln Sie im Admin Center zur Seite **Gruppen** > [Gruppen](https://admin.microsoft.com/adminportal/home#/groups). 
    
    2. Suchen Sie die DG, der Sie den externen Benutzer hinzufügen möchten, und wählen Sie sie aus, um das Bearbeitungsdialogfeld zu öffnen.
    
    3. Wählen Sie auf der Registerkarte **Mitglieder** die Option **Alle anzeigen und Mitglieder verwalten** aus. 
    
    4. Wählen Sie **Mitglieder hinzufügen** aus.
    
    5. Wählen Sie den E-Mail-Kontakt aus, den Sie im vorherigen Schritt erstellt haben, und wählen Sie dann **Speichern** aus.
    
Wenn Ihre externen Benutzer nach dem Ausführen dieser Schritte keine E-Mails an die DG senden können oder keine E-Mails von dieser erhalten, kann es sein, dass die DG so gekennzeichnet ist, dass nur E-Mails von internen Benutzern zugelassen werden. Sie können diese Konfiguration überprüfen und nach den Anweisungen [hier](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)beheben.
  
 **Hinweis:** Diese Anweisungen gelten nicht, wenn der Typ Ihrer Gruppe "Microsoft 365 Gruppe" anstelle von "Verteilergruppe" ist. Wenn dies der Fall ist, können Sie den externen Benutzer direkt aus Outlook der Gruppe hinzufügen. Ausführliche Informationen zu gästen Microsoft 365 Gruppen sowie Anweisungen zum Hinzufügen externer Gäste finden Sie in [diesem Artikel.](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx)
  