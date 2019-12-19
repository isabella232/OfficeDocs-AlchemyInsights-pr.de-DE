---
title: Fehler beim Validieren des Zugriffstoken Fehlers beim on-Boarding von Desktop Analytics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741178"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler beim Validieren des Zugriffstokens beim Desktop Analyse-Onboarding

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. In der Regel wird durch das Aktualisieren der Seite das Token aktualisiert. Dieses Problem kann jedoch bestehen bleiben, wenn auf das Konto, das für die on-Board-Desktop Analyse verwendet wird, bedingte Zugriffsrichtlinien angewendet werden. Sie können die Azure AD Anmelde Protokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das für das Onboarding von Desktop Analytics verwendete Konto vorliegen.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Planen der Bereitstellung für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).