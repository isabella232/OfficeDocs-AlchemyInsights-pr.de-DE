---
title: Fehler beim Überprüfen des Zugriffstokenfehlers beim Einsteigen in Desktop Analytics
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
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813687"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Fehler "Fehler beim Überprüfen des Zugriffstokens" beim Desktop Analytics-Onboarding

Dieser Fehler wird normalerweise beim Ablauf des Authentifizierungstokens beobachtet. In der Regel aktualisiert das Aktualisieren der Seite das Token. Dieses Problem kann jedoch bestehen bleiben, wenn Richtlinien für bedingten Zugriff auf das Konto angewendet werden, das für die on-board-Desktopanalyse verwendet wird. Sie können die Azure AD-Anmeldeprotokolle im Azure-Portal überprüfen, um zu sehen, ob für das Konto, das für das Desktop Analytics-Onboarding verwendet wird, Anmeldefehler gibt.

Weitere Informationen zum bedingten Zugriff finden Sie unter [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).