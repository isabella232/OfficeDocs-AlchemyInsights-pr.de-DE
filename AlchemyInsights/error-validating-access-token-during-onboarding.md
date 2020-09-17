---
title: Fehler beim Validieren des Zugriffstoken Fehlers beim on-Boarding von Desktop Analytics
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 45c6fb1a1632799a07c028c0791b6b8e77635293
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783550"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler beim Validieren des Zugriffstokens beim Desktop Analyse-Onboarding

Dieser Fehler wird normalerweise beobachtet, wenn das Authentifizierungstoken abläuft. In der Regel wird durch das Aktualisieren der Seite das Token aktualisiert. Dieses Problem kann jedoch bestehen bleiben, wenn auf das Konto, das für die on-Board-Desktop Analyse verwendet wird, bedingte Zugriffsrichtlinien angewendet werden. Sie können die Azure AD Anmelde Protokolle im Azure-Portal überprüfen, um festzustellen, ob Anmeldefehler für das für das Onboarding von Desktop Analytics verwendete Konto vorliegen.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Planen der Bereitstellung für bedingten Zugriff](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).