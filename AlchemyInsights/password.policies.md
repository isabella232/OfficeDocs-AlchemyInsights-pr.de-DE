---
title: Kennwortrichtlinien
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "9277"
ms.openlocfilehash: 12751288d04a2ec5993bf4a546b7d0c862f8f171f5bfd7a337cb79cb95792056
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040829"
---
# <a name="password-policies"></a>Kennwortrichtlinien

**Ich habe Probleme mit der Kennwortrichtlinie für einen Benutzer**

- Die Kennwortrichtlinie für einen Benutzer hängt davon ab, ob der Benutzer nur in der Cloud oder lokal ist.
- Nur Cloudbenutzer müssen ein Kennwort auswählen, das die Anforderungen in diesem Artikel erfüllt: [Kennwortrichtlinien, die nur für Cloudbenutzerkonten gelten](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#password-policies-that-only-apply-to-cloud-user-accounts)
- Lokale Benutzer müssen ein Kennwort auswählen, das die lokalen Anforderungen erfüllt. Wenn ein lokaler Benutzer sein Kennwort nicht festlegen kann, überprüfen Sie Ihre lokalen Anforderungen.

**Ich weiß nicht, wie Kennwortablaufrichtlinien festgelegt oder überprüft werden**

- Sie können die Ablaufrichtlinie für Cloudbenutzer in Ihrem Mandanten mithilfe von PowerShell festlegen und überprüfen. Folgen Sie den Anweisungen in diesem Artikel: [Festlegen oder Überprüfen der Kennwortrichtlinien mithilfe von PowerShell](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- Die Kennwortablaufrichtlinie für lokale Benutzer wird in Ihrem lokalen AD festgelegt.

**Weitere hilfreiche Links:**
- [Erste Schritte mit der Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#set-or-check-the-password-policies-by-using-powershell)
- [Problembehandlung bei der vom Administrator initiierten Kennwortzurücksetzung](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshoot-the-password-reset-portal)
