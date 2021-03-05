---
title: Problembehandlung für SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 85bfc812dcffce008a6fa5394a6069bd64c514d6
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50428693"
---
# <a name="troubleshoot-sspr"></a>Problembehandlung für SSPR

**Probleme beim Konfigurieren der Kennwortzurücksetzung**

- Wenn Sie Administrator sind und suchen, wie Sie die Self-Service-Kennwortzurücksetzung aktivieren möchten, lesen Sie Lernprogramm aktivieren [SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr), um die Kennwortzurücksetzung für Ihre Organisation zu konfigurieren. Möglicherweise möchten Sie auch die [Lizenzierungsanforderungen überprüfen.](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support) In Ihrer Organisation muss mindestens eine Lizenz zugewiesen sein.
    - **Nur Cloudbenutzer** – Office 365 (O365) kostenpflichtige SKU oder Azure AD Basic
    - **Cloud- und/oder lokale Benutzer** – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)
- Weitere Fragen zur Self-Service-Kennwortzurücksetzung finden Sie [in den häufig gestellten Fragen](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support).

**Ich bekommt eine Fehlermeldung**

Lesen Sie diesen Artikel, um häufige Fehler und deren Lösungen zu finden: Problembehandlung bei der [Self-Service-Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich habe ein Problem mit meiner Kennwortzurücksetzungsrichtlinie**

- Wenn Ihre Kennwortzurücksetzungsrichtlinie nicht wie erwartet ausgeführt wird oder Wenn Sie Fragen zu Kennwortzurücksetzungsrichtlinien haben, lesen Sie diesen Artikel: [Kennwortrichtlinien](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)und Einschränkungen in Azure Active Directory .
- Richtlinien für die Kennwortzurücksetzung gelten nicht für Administratoren. Microsoft erzwingt eine starke standardmäßige Zwei-Tore-Kennwortzurücksetzungsrichtlinie für alle Azure-Administratorrolle. Stellen Sie sicher, dass Sie mit einem Benutzer testen, der kein Administrator ist. Weitere Informationen zur Administratorzurücksetzungsrichtlinie finden Sie in diesem Artikel: Unterschiede zwischen [den Richtlinien für die Administratorzurücksetzung](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences).

**Ich möchte nicht, dass meine Benutzer zusätzliche Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

Sie können Daten (E-Mail- und Telefonattribute) für Ihre Benutzer vorab mithilfe einer API, PowerShell oder Azure AD Connect auffüllen. So erfahren Sie, wie Sie lesen:

- [Bereitstellen der Kennwortzurücksetzung, ohne dass Benutzer sich registrieren müssen](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [Welche Daten bei der Kennwortzurücksetzung verwendet werden](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**Ich möchte, dass meine Benutzer ihre zusätzlichen Sicherheitsinformationen für die Kennwortzurücksetzung registrieren.**

1. Lassen Sie Ihre Benutzer ihre Sicherheitsinformationen für die Self-Service-Kennwortzurücksetzung registrieren, indem sie sie [an](https://mysignins.microsoft.com/security-info)aka.ms/ssprsetup.
1. Nachdem Daten für den Benutzer (vom Benutzer oder vom Administrator) aufgefüllt wurden, müssen Sie den Benutzer an aka.ms/sspr damit Ihre Benutzer ihre eigenen Kennwörter zurücksetzen können. [](https://passwordreset.microsoftonline.com/)
1. Wenn Benutzer weiterhin Probleme haben, handelt es sich höchstwahrscheinlich um **Synchronisierte** Benutzer mit Verbund- oder **Kennworthash.** Dies bedeutet, dass es wahrscheinlich ein Problem mit dem Kennwortrückschreibendienst gibt.