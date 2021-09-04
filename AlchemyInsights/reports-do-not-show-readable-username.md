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
- "9008619"
ms.openlocfilehash: 1741aab633b28a9c991a3e4a972f85a67c26705e
ms.sourcegitcommit: 1761960d03b3df7783b744ee539a7e6dbabae90c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/03/2021
ms.locfileid: "58884044"
---
# <a name="reports-in-microsoft-365-admin-center-do-not-show-readable-username"></a>Berichte im Microsoft 365 Admin Center zeigen keinen lesbaren Benutzernamen an

Berichte im Microsoft 365 Admin Center zeigen keine Benutzernamen, sondern alphanumerische Werte wie B2BC6C15BB9FCDEA71E5CD302D228CC8 an.

Dies ist ein erwartetes Verhalten und wurde im Nachrichtencenter kommuniziert (MC275344, veröffentlicht am 3. August 2021). 

Globale Administratoren können diese Änderung für ihren Mandanten rückgängig machen und identifizierbare Benutzerinformationen anzeigen, sollten die Datenschutzpraktiken ihrer Organisation dies zulassen. So machen Sie die Änderung für den Mandanten rückgängig:

1. Wechseln Sie im Admin Center zu **Einstellungen** > **Organisationseinstellungsdienste** > **Dienste** und wählen Sie **"Berichte"** aus. 
1. Wählen Sie unter **"Auswählen, wie Benutzerinformationen angezeigt werden sollen"** die Option **"Identifizierbare Benutzerinformationen in Berichten anzeigen"** und führen Sie den Bericht dann erneut aus.