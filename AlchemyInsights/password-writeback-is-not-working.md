---
title: Kennwortrückschreiben funktioniert nicht
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232720"
---
# <a name="password-writeback-is-not-working"></a>Kennwortrückschreiben funktioniert nicht

**Ich habe Probleme beim Konfigurieren des Kennwortrückschreibens**

- Kennwortrückschreiben ist ein Premium-Feature.
- Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen kennen:
  - Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein.
  - **Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365)-SKU oder Azure AD Basic
  - **Cloud- und/oder** lokale Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
    - Weitere Informationen zu Den Lizenzierungsanforderungen finden Sie unter Lizenzierungsanforderungen für die [Self-Service-Kennwortzurücksetzung in Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- Sie verfügen über mindestens ein Administratorkonto und ein Testbenutzerkonto mit einer der entsprechenden Lizenz.
- Sie müssen Azure AD Connect mit dem primären Domänencontrolleremulator verbinden, damit das Kennwortrückschreiben funktioniert. Sie können Azure AD Connect für die Verwendung eines  primären Domänencontrollers konfigurieren, indem Sie mit der rechten Maustaste auf die Eigenschaften des Active Directory-Synchronisierungsconnector klicken und dann **Verzeichnispartitionen konfigurieren.** Suchen Sie von dort aus nach **dem** Abschnitt mit den Einstellungen für die Domänencontrollerverbindung, und aktivieren Sie das Kontrollkästchen mit der Bezeichnung **"Nur bevorzugte Domänencontroller verwenden".**
  > [!NOTE]
  > Wenn es sich bei dem bevorzugten DC nicht um einen PDC-Emulator handelt, kontaktiert Azure AD Connect weiterhin das PDC für das Kennwortrückschreiben.
- Die Kennwortzurücksetzung wurde in Ihrem Mandanten konfiguriert und aktiviert. Weitere Informationen finden Sie unter "Aktivieren der Benutzer [zum Zurücksetzen ihrer Azure AD-Kennwörter".](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)
- Stellen Sie sicher, dass das Administratorkonto, das zum Aktivieren des Kennwortrückschreibens verwendet wird, ein Cloudadministratorkonto ist (erstellt in Azure AD und nicht in der lokalen AD-Bereitstellung)
- Sie verfügen über eine lokale Ad-Bereitstellung mit einer oder mehreren Gesamtstrukturen, in der Windows Server 2008 R2, Windows Server 2012 oder Windows Server 2012 R2 ausgeführt wird, in der die neuesten Service Packs installiert sind.
- Sie haben das Azure AD Connect-Tool installiert und Ihre AD-Umgebung für die Synchronisierung mit der Cloud vorbereitet. Stellen Sie vor dem Testen des Kennwortrückschreibens sicher, dass Sie zuerst einen vollständigen Import und eine vollständige Synchronisierung aus AD und Azure AD in Azure AD Connect abschließen.
- Weitere Informationen finden Sie unter einer vollständigen Synchronisierung [und einem vollständigen Import in Azure AD Connect](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**I'm having a problem with password writeback connectivity**

1. Herunterladen und Aktivieren der neuesten Version von [Azure AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)
2. Firewallkonfiguration: Das Azure AD -Connect-Tool (1.1.443 und höher) benötigt **ausgehenden HTTPS-Zugriff** auf:
    - passwordreset.microsoftonline.com
    - servicebus.windows.networks
3. Zulassen, dass Leerlaufverbindungen mindestens 2-3 Minuten lang bestehen bleiben

**Ich habe weiterhin Probleme mit dem Kennwortrückschreiben**

- Wenn sie weiterhin Probleme haben, versuchen Sie, den Kennwortrückschreibendienst im Azure AD -Connect-Tool zu deaktivieren und erneut zu aktivieren.
- Weitere Informationen finden Sie unter Deaktivieren und erneutes Aktivieren [des Kennwortrückschreibens.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
