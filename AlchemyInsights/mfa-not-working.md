---
title: Probleme mit MFA
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 63f7d676-7cd9-4549-ba84-c3a8a7867f63
ms.custom:
- "2417"
- "9000557"
ms.openlocfilehash: 718af9bfbc0a64cdfc96528e5062fb96c8d0f2d3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47755130"
---
# <a name="issues-with-azure-mfa"></a>Probleme mit Azure MFA
Es gibt einige Dinge, die überprüft werden müssen, wenn sich Benutzer nicht mit mehrstufiger Authentifizierung (MFA) anmelden können.

1. Der betroffene Benutzer wird möglicherweise in Azure Active Directory-Portal blockiert. Wenn dies der Fall ist, werden Authentifizierungsversuche für diesen bestimmten Benutzer automatisch verweigert. [Führen Sie die Schritte in diesem Artikel aus, um die Blockierung aufzuheben.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-mfasettings#block-and-unblock-users)

2. Wenn die Blockierung des Benutzers aufgehoben wurde oder der Benutzer nicht blockiert ist, können Sie versuchen, MFA für den Benutzer zurückzusetzen, und Sie werden den Registrierungsprozess erneut durchlaufen. [Führen Sie die Schritte in diesem Artikel aus.](https://docs.microsoft.com/azure/active-directory/authentication/howto-mfa-userdevicesettings#require-users-to-provide-contact-methods-again)

Wenn Sie das erste Mal MFA aktiviert haben und sich Ihre Benutzer nicht für Clients wie Outlook, Skype usw. anmelden können, die möglicherweise Adal (Active Directory Authentifizierungsbibliothek) in Ihrem O365-Abonnement nicht aktiviert sind. In diesem Fall müssen Sie eine Verbindung mit Exchange Online PowerShell herstellen und dieses Cmdlet ausführen:  *festlegen-OrganizationConfig-OAuth2ClientProfileEnabled: $true*