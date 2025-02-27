---
title: Hinzufügen einer Unterdomäne
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
- "7"
- "13902"
ms.openlocfilehash: ea39984a54a15ae6167363eb5855943c8ab1120d
ms.sourcegitcommit: a097d1f8915a31ed8460b5b68dccc8d87e563cc0
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/22/2021
ms.locfileid: "59475953"
---
# <a name="adding-a-sub-domain"></a>Hinzufügen einer Unterdomäne

Unterdomänen können derselben oder einem anderen Mandanten als der übergeordneten Domäne hinzugefügt werden. In beiden Fällen müssen Sie Ihre eigenen DNS-Einstellungen auf der Website Ihrer Registrierungsstelle verwalten. Wenn Sie Microsoft die Verwaltung Ihrer DNS-Einstellungen mit NS-Einträgen ermöglicht haben oder wenn Sie die Domäne von Microsoft gekauft haben, können Sie keine Unterdomänen hinzufügen, ohne dies zuerst zu ändern.

Fügen Sie zuerst die übergeordnete Domäne und dann die Unterdomäne hinzu. Wenn sich die Unterdomäne im selben Mandanten befindet, ist keine zusätzliche Überprüfung erforderlich. Wenn Sie die Unterdomäne zu einem separaten Mandanten hinzufügen, ist der DNS-TXT-Eintrag für die Besitzüberprüfung erforderlich, bevor die Domäne und die zusätzlichen DNS-Einträge für die ausgewählten Dienste hinzugefügt werden.

- Um eine Domäne oder Unterdomäne hinzuzufügen, folgen Sie dem Assistenten zum Hinzufügen von [Domänen,](https://admin.microsoft.com/Adminportal#/Domains/Wizard)oder fügen Sie die Domäne oder Unterdomäne manuell hinzu, indem Sie zu   >  **"Domänen**  >  **hinzufügen"** wechseln.

Bei Bedarf:

- Um zu ändern, wer Ihre DNS-Einstellungen für eine vorhandene Domäne verwaltet, wechseln Sie zu **Einstellungen**  >  [**Domänen,**](https://admin.microsoft.com/Adminportal/Home#/Domains)aktivieren Sie das Kontrollkästchen neben der Domäne, und wählen Sie dann **DNS verwalten** aus. Wählen Sie im Assistenten Ihre **eigenen DNS-Einträge hinzufügen aus,** und schließen Sie den Assistenten ab.
- Um einer von Microsoft erworbenen Domäne Unterdomänen hinzuzufügen, übertragen Sie die Domäne zuerst an eine andere Registrierungsstelle, und nehmen Sie dann die oben beschriebene Änderung vor, um Ihre eigenen DNS-Einträge zu verwalten. Anweisungen finden Sie unter [Übertragen einer Domäne von Microsoft auf einen anderen Host.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/transfer-a-domain-from-microsoft-to-another-host)
- Wenn Sie eine Fehlermeldung erhalten, dass Ihre Domäne bereits von anderen Mitgliedern oder Personen in Ihrer Organisation verwendet wird, müssen Sie zuerst dieses nicht verwaltete Konto übernehmen, bevor Sie die Domäne verwenden. Anweisungen finden Sie unter [Übernehmen eines nicht verwalteten Verzeichnisses als Administrator in Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/enterprise-users/domains-admin-takeover)
