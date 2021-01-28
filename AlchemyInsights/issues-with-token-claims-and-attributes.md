---
title: Probleme mit Tokenansprüchen und -attributen
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
- "9004347"
- "7761"
ms.openlocfilehash: 4c12f768ab4bf4547f48abc19736743fa555c477
ms.sourcegitcommit: c1c6047ec467853dc823a17b02c461a6a476406d
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50029987"
---
# <a name="issues-with-token-claims-and-attributes"></a>Probleme mit Tokenansprüchen und -attributen

**Aktualisieren, Konfigurieren oder Entfernen von Tokenansprüchen**

1. Mithilfe von Azure Active Directory (Azure AD) können Sie den Anspruchstyp für den Rollenanspruch [im](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) Antworttoken anpassen, das Sie erhalten, nachdem Sie eine App autorisiert haben.
2. Anwendungsentwickler können optionale Ansprüche in ihren Azure AD-Anwendungen verwenden, um anzugeben, welche Ansprüche sie in Token wünschen, die an ihre Anwendung gesendet werden. Weitere Informationen finden Sie unter [Bereitstellen optionaler Ansprüche für Ihre App.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)
3. [Konfigurieren von Gruppenansprüchen für Anwendungen mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).
4. Wenn Sie nahtloses einmaliges Anmelden in Ihrer Anwendung verwenden, lesen Sie die Informationen zum Anpassen von Ansprüchen, die [im SAML-Token für Unternehmensanwendungen ausgestellt wurden.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)

**Zuordnung von Anspruchsattributen**

1. Informationen zum Konfigurieren der [Anspruchszuordnungsrichtlinie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)mithilfe von PowerShell finden Sie unter Anpassen von Ansprüchen, die in Token für eine bestimmte App in einem Mandanten ausgegeben werden (Vorschau).
2. Verzeichnisschemaerweiterungsattribute bieten eine Möglichkeit, zusätzliche Daten in Azure Active Directory auf Benutzerobjekten und anderen Verzeichnisobjekten wie Gruppen, Mandantendetails, Dienstprinzipale zu speichern. Nur Erweiterungsattribute für Benutzerobjekte können zum Aussenten von Ansprüchen an Anwendungen verwendet werden. [Die Verwendung von Verzeichnisschemaerweiterungsattributen in](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) Ansprüchen beschreibt, wie Verzeichnisschemaerweiterungsattribute zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen verwendet werden.

Weitere Informationen zu Tokenansprüchen finden Sie unter:

- [Ansprüche in Zugriffstoken](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [Ansprüche in id_token](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- [Ansprüche,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) die Sie in von Azure AD B2C ausgestellten ID- und Zugriffstoken erwarten können
- [SamL-Token-Anspruchsreferenz](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
