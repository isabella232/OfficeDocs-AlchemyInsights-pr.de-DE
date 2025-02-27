---
title: Problem beim Öffnen oder Herunterladen von Dateien in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: cb32085d13cbb5f609b887fc2b63e7af5ae056eb49c121a21722a147c67e30d8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028255"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>Problem beim Öffnen oder Herunterladen von Dateien in Yammer

Das klassische Yammer unterstützt mehrere Optionen für das Hochladen von Dateien in Nachrichten und Gruppen. Je nach Netzwerkkonfiguration sind Dateien standardmäßig in SharePoint gespeichert.

Die Dateiauswahl im neuen Yammer unterstützt noch nicht alle Optionen, die im klassischen Yammer zur Verfügung stehen. Ein zukünftiges Update wird weitere Features hinzufügen. Weitere Informationen hierzu finden Sie unter [Anfügen einer Datei oder eines Bilds an einen Beitrag in einer Yammer-Unterhaltung](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).

**Datei kann nicht geöffnet oder heruntergeladen werden**  

Eine Datei kann in Yammer hochgeladen werden, aber zusätzlich auf eine Datei in SharePoint Online verlinkt sein. Zur Problembehandlung müssen Sie zuerst den Speicherort der Datei ermitteln. Wenn die Datei in Yammer hochgeladen wurde, weist sie eine *.yammer.com-URL auf. Stellen Sie sicher, dass erforderliche URLs und IP-Adressen nicht blockiert werden. Weitere Informationen hierzu finden Sie im Blogbeitrag [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).

Überprüfen Sie, ob ein Benutzer, der auch ein globaler Administrator ist, die Datei herunterladen kann. Ist die Datei privat, müssen Sie möglicherweise den Modus für private Inhalte verwenden. Weitere Informationen finden Sie unter [Überwachen privater Inhalte in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).  

**Gäste und Dateien auf Yammer-Netzwerkebene in SharePoint Online**  

[Gäste auf Yammer-Netzwerkebene](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) verwenden kein Azure AD B2B und sind für den Yammer-Dienst interne Benutzer, daher können Sie auf in SharePoint gespeicherte Yammer-Dateien nicht zugreifen. Erstellen Sie einen externen AAD-B2B-Benutzer, der unter Verwendung dieser Identität auf Dokumentbibliotheken in SharePoint Online zugreifen kann. Informationen zur künftigen Azure AD B2B-Gastunterstützung in Yammer finden Sie unter [Business-to-Business (B2B) – Gast Support in Yammer, Vorschau – Kundenbedingungen und häufig gestellte Fragen (FAQ)](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).