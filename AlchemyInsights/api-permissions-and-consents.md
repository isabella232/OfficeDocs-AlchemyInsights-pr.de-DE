---
title: API-Berechtigungen und Zustimmung
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/25/2021
ms.locfileid: "49951894"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="03ab7-102">API-Berechtigungen und Zustimmung</span><span class="sxs-lookup"><span data-stu-id="03ab7-102">API permissions and consent</span></span>

<span data-ttu-id="03ab7-103">Anwendungen, die mit Microsoft Identity Platform integriert werden, folgen einem Autorisierungsmodell, mit dem Benutzer und Administratoren steuern können, wie auf Daten zugegriffen werden kann.</span><span class="sxs-lookup"><span data-stu-id="03ab7-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="03ab7-104">Die Implementierung des Autorisierungsmodells wurde auf dem Microsoft Identity Platform-Endpunkt aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="03ab7-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="03ab7-105">Es ändert die Art und Weise, wie eine App mit der Microsoft Identity Platform interagieren muss.</span><span class="sxs-lookup"><span data-stu-id="03ab7-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="03ab7-106">[Berechtigungen und Zustimmungen im Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) Platform-Endpunkt umfassen die grundlegenden Konzepte dieses Autorisierungsmodells, einschließlich Bereiche, Berechtigungen und Zustimmung.</span><span class="sxs-lookup"><span data-stu-id="03ab7-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="03ab7-107">Das [Azure Active Directory (Azure AD)-Zustimmungsframework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) erleichtert die Entwicklung von mehr mandanteneigenen Web- und systemeigenen Clientanwendungen.</span><span class="sxs-lookup"><span data-stu-id="03ab7-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="03ab7-108">Diese Anwendungen ermöglichen die Anmeldung über Benutzerkonten von einem Azure AD-Mandanten, der sich von dem, in dem die Anwendung registriert ist, unterscheiden.</span><span class="sxs-lookup"><span data-stu-id="03ab7-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="03ab7-109">Sie müssen möglicherweise zusätzlich zu Ihren eigenen Web-APIs auch auf Web-APIs wie die Microsoft Graph-API (für den Zugriff auf Azure AD, Intune und Dienste in Microsoft 365) und die APIs anderer Microsoft-Dienste zugreifen.</span><span class="sxs-lookup"><span data-stu-id="03ab7-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

