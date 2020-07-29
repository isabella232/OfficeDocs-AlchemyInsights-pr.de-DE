---
title: Löschen eines privaten Teams-Kanals
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3781"
- "9001223"
ms.openlocfilehash: 2ee998f0c70973645c273a2a6609af2420a4f74b
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45431616"
---
# <a name="delete-a-teams-private-channel"></a>Löschen eines privaten Teams-Kanals

Microsoft ist sich eines Problems beim Löschen eines privaten Teams-Kanals bewusst, wenn Sie für die zugrunde liegende SharePoint-Site SharePoint-Aufbewahrungsrichtlinien aktiviert haben. Microsoft arbeitet derzeit an einer Lösung. In der Zwischenzeit können Sie folgenden Problemumgehungen verwenden, um den privaten Kanal zu löschen.

**Schließen Sie die Team-/Websitesammlung aus der SharePoint-Aufbewahrungsrichtlinie aus.**

1. Wechseln Sie zum Office 365-Verwaltungsportal, und wählen Sie im linken Navigationsbereich **Alle anzeigen** aus.
2. Wechseln Sie unter **Admin Center** zu **Security & Compliance** > **Verhinderung von Datenverlust** > **Richtlinie**.
3. Identifizieren Sie eine Richtlinie, die für SharePoint-Sites gilt, und ändern Sie die Richtlinie so, dass die SharePoint-Site für das Team, das den privaten Kanal enthält, NICHT unter der Aufbewahrungsrichtlinie enthalten ist.
4. Speichern Sie die Richtlinie.
    Es kann bis zu 24 Stunden dauern, bis Richtlinieneinstellungen wirksam werden.
    Nachdem die Site ausgeschlossen wurde, können Sie den privaten Kanal löschen.  
    
***Möglicherweise können*** Sie den privaten Kanal löschen, indem Sie Microsoft Teams auf Ihrem Android-Gerät verwenden. 

Verwandte SharePoint-Informationen finden Sie unter [Elemente in SharePoint Online oder OneDrive for Business können nicht gelöscht werden](https://docs.microsoft.com/alchemyinsights/retention-policy-ediscovery-hold).