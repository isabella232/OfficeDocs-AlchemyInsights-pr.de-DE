---
title: Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/02/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13809"
- "13810"
- "13812"
- "9008619"
ms.openlocfilehash: 16aa4f052c934421423c73244f03a20aa38e4785
ms.sourcegitcommit: 76c61dec041b93d0039764fae38107108da324aa
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2021
ms.locfileid: "58896347"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an

Berichte im Microsoft 365 Admin Center zeigen keine Benutzernamen an, sondern Alpha-Numerische Werte wie B2BC6C15BB9FCDEA71E5CD302D228CC8.

Dies ist das erwartete Verhalten und wurde im Nachrichtencenter kommuniziert (MC275344, veröffentlicht am 3. August 2021). 

Globale Administratoren können diese Änderung für ihren Mandanten rückgängig machen und identifizierbare Benutzerinformationen anzeigen, wenn die Datenschutzpraktiken ihrer Organisation dies zulassen. So machen Sie die Änderung für den Mandanten rückgängig:

1. Wechseln Sie im Admin Center zu **Einstellungen** > **Organisationseinstellungsdienste,** > [**Dienste**](https://admin.microsoft.com/Adminportal/Home#/Settings/Services) und wählen Sie **Berichte** aus. 
1. Wählen Sie unter **Auswählen, wie Benutzerinformationen angezeigt werden sollen** die Option **Identifizierbare Benutzerinformationen in Berichten anzeigen** aus, und führen Sie dann den Bericht erneut aus.