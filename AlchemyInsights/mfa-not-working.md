---
title: Probleme mit MFA
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 2fed99ebf553a9bfda436d81797c841987759e98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51810483"
---
# <a name="issues-with-azure-mfa"></a>Probleme mit Azure MFA
Es gibt einige Dinge, die überprüft werden müssen, ob sich Benutzer nicht mit der mehrstufigen Authentifizierung (MFA) anmelden können.

1. Der betroffene Benutzer wird möglicherweise im Azure Active Directory-Portal blockiert. In diesem Fall werden Authentifizierungsversuche für den jeweiligen Benutzer automatisch verweigert. [Führen Sie die Schritte in diesem Artikel aus, um die Blockierung zu aufheben.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Wenn die Sperrung des Benutzers nicht hilfreich war oder der Benutzer nicht blockiert ist, können Sie versuchen, MFA für den Benutzer zurückzusetzen, und er wird den Registrierungsprozess erneut durchgehen. [Führen Sie die Schritte in diesem Artikel aus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Wenn Dies das erste Mal ist, dass Sie MFA aktiviert haben und Sich Ihre Benutzer nicht bei Nicht-Browser-Clients wie Outlook, Skype usw. anmelden können, ist möglicherweise ADAL (Active Directory Authentication Library) für Ihr O365-Abonnement nicht aktiviert. In diesem Fall müssen Sie eine Verbindung mit Exchange Online Powershell herstellen und dieses Cmdlet ausführen:  *Set-OrganizationConfig -OAuth2ClientProfileEnabled:$true*