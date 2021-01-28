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
# <a name="issues-with-token-claims-and-attributes"></a><span data-ttu-id="fc695-102">Probleme mit Tokenansprüchen und -attributen</span><span class="sxs-lookup"><span data-stu-id="fc695-102">Issues with Token Claims and Attributes</span></span>

<span data-ttu-id="fc695-103">**Aktualisieren, Konfigurieren oder Entfernen von Tokenansprüchen**</span><span class="sxs-lookup"><span data-stu-id="fc695-103">**Update, configure or remove token claims**</span></span>

1. <span data-ttu-id="fc695-104">Mithilfe von Azure Active Directory (Azure AD) können Sie den Anspruchstyp für den Rollenanspruch [im](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) Antworttoken anpassen, das Sie erhalten, nachdem Sie eine App autorisiert haben.</span><span class="sxs-lookup"><span data-stu-id="fc695-104">By using Azure Active Directory (Azure AD), you can [customize the claim type for the role claim](https://docs.microsoft.com/azure/active-directory/develop/active-directory-enterprise-app-role-management) in the response token that you receive after you authorize an app.</span></span>
2. <span data-ttu-id="fc695-105">Anwendungsentwickler können optionale Ansprüche in ihren Azure AD-Anwendungen verwenden, um anzugeben, welche Ansprüche sie in Token wünschen, die an ihre Anwendung gesendet werden.</span><span class="sxs-lookup"><span data-stu-id="fc695-105">Application developers can use optional claims in their Azure AD applications to specify which claims they want in tokens sent to their application.</span></span> <span data-ttu-id="fc695-106">Weitere Informationen finden Sie unter [Bereitstellen optionaler Ansprüche für Ihre App.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims)</span><span class="sxs-lookup"><span data-stu-id="fc695-106">For more information, see [Provide optional claims to your app](https://docs.microsoft.com/azure/active-directory/develop/active-directory-optional-claims).</span></span>
3. <span data-ttu-id="fc695-107">[Konfigurieren von Gruppenansprüchen für Anwendungen mit Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span><span class="sxs-lookup"><span data-stu-id="fc695-107">[Configure group claims for applications with Azure Active Directory](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-fed-group-claims).</span></span>
4. <span data-ttu-id="fc695-108">Wenn Sie nahtloses einmaliges Anmelden in Ihrer Anwendung verwenden, lesen Sie die Informationen zum Anpassen von Ansprüchen, die [im SAML-Token für Unternehmensanwendungen ausgestellt wurden.](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization)</span><span class="sxs-lookup"><span data-stu-id="fc695-108">If using Seamless Single Sign-on in your application, see [customize claims issued in the SAML token for enterprise applications](https://docs.microsoft.com/azure/active-directory/develop/active-directory-saml-claims-customization).</span></span>

<span data-ttu-id="fc695-109">**Zuordnung von Anspruchsattributen**</span><span class="sxs-lookup"><span data-stu-id="fc695-109">**Claims Attribute Mapping**</span></span>

1. <span data-ttu-id="fc695-110">Informationen zum Konfigurieren der [Anspruchszuordnungsrichtlinie](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping)mithilfe von PowerShell finden Sie unter Anpassen von Ansprüchen, die in Token für eine bestimmte App in einem Mandanten ausgegeben werden (Vorschau).</span><span class="sxs-lookup"><span data-stu-id="fc695-110">To configure claims mapping policy using PowerShell, see [Customize claims emitted in tokens for a specific app in a tenant (Preview)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-claims-mapping).</span></span>
2. <span data-ttu-id="fc695-111">Verzeichnisschemaerweiterungsattribute bieten eine Möglichkeit, zusätzliche Daten in Azure Active Directory auf Benutzerobjekten und anderen Verzeichnisobjekten wie Gruppen, Mandantendetails, Dienstprinzipale zu speichern.</span><span class="sxs-lookup"><span data-stu-id="fc695-111">Directory schema extension attributes provide a way to store additional data in Azure Active Directory on user objects and other directory objects such as groups, tenant details, service principals.</span></span> <span data-ttu-id="fc695-112">Nur Erweiterungsattribute für Benutzerobjekte können zum Aussenten von Ansprüchen an Anwendungen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fc695-112">Only extension attributes on user objects can be used for emitting claims to applications.</span></span> <span data-ttu-id="fc695-113">[Die Verwendung von Verzeichnisschemaerweiterungsattributen in](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) Ansprüchen beschreibt, wie Verzeichnisschemaerweiterungsattribute zum Senden von Benutzerdaten an Anwendungen in Tokenansprüchen verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="fc695-113">[Using directory schema extension attributes in claims](https://docs.microsoft.com/azure/active-directory/develop/active-directory-schema-extensions) describes how to use directory schema extension attributes for sending user data to applications in token claims.</span></span>

<span data-ttu-id="fc695-114">Weitere Informationen zu Tokenansprüchen finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="fc695-114">For more information on token claims, see:</span></span>

- [<span data-ttu-id="fc695-115">Ansprüche in Zugriffstoken</span><span class="sxs-lookup"><span data-stu-id="fc695-115">Claims in access tokens</span></span>](https://docs.microsoft.com/azure/active-directory/develop/access-tokens#claims-in-access-tokens)
- [<span data-ttu-id="fc695-116">Ansprüche in id_token</span><span class="sxs-lookup"><span data-stu-id="fc695-116">Claims in an id_token</span></span>](https://docs.microsoft.com/azure/active-directory/develop/id-tokens#claims-in-an-id_token)
- <span data-ttu-id="fc695-117">[Ansprüche,](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) die Sie in von Azure AD B2C ausgestellten ID- und Zugriffstoken erwarten können</span><span class="sxs-lookup"><span data-stu-id="fc695-117">[Claims](https://docs.microsoft.com/azure/active-directory-b2c/tokens-overview#claims) that you can expect in ID tokens and access tokens issued by Azure AD B2C</span></span>
- [<span data-ttu-id="fc695-118">SamL-Token-Anspruchsreferenz</span><span class="sxs-lookup"><span data-stu-id="fc695-118">SAML token claims reference</span></span>](https://docs.microsoft.com/azure/active-directory/develop/reference-saml-tokens)
