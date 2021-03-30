---
title: Single-Sign für Azure Active Directory-beigetretene Geräte aktiviert
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403797"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="ddbf7-102">Einmaliges Anmelden für Azure Active Directory-beigetretene Geräte</span><span class="sxs-lookup"><span data-stu-id="ddbf7-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="ddbf7-103">Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre mit der AD-Domäne beigetretenen Computer zu Azure AD hinzufügen möchten, können Sie dies erreichen, indem Sie azure AD hybrid beitreten.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="ddbf7-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="ddbf7-105">Konfigurieren von In Azure AD beigetretenen Geräten für lokale Single-Sign On mithilfe von Windows Hello for Business</span><span class="sxs-lookup"><span data-stu-id="ddbf7-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="ddbf7-106">**Probleme mit dem primären Aktualisierungstoken (Primary Refresh Token, PRT)** Ein primäres Aktualisierungstoken (Primary Refresh Token, PRT) ist ein Schlüsselartefakte der Azure AD-Authentifizierung auf Windows 10-, Windows Server 2016- und höher-, iOS- und Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="ddbf7-107">Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Microsoft first party ausgegeben wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die Anwendungen zu aktivieren, die auf diesen Geräten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="ddbf7-108">[Unter Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)stellen wir Details dazu zur Verfügung, wie ein PRT auf Windows 10-Geräten ausgegeben, verwendet und geschützt wird.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="ddbf7-109">**WamDefaultSet: JA und AzureADPrt: JA** Diese Felder geben an, ob sich der Benutzer erfolgreich bei Azure AD authentifiziert hat, wenn er sich beim Gerät anmeldet.</span><span class="sxs-lookup"><span data-stu-id="ddbf7-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="ddbf7-110">Wenn die Werte **NO sind,** kann dies fällig sein:</span><span class="sxs-lookup"><span data-stu-id="ddbf7-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="ddbf7-111">Ungültiger Speicherschlüssel im TPM, das dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie den KeySignTest, während Sie mit erhöhten Rechten ausgeführt werden).</span><span class="sxs-lookup"><span data-stu-id="ddbf7-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="ddbf7-112">Alternative Anmelde-ID</span><span class="sxs-lookup"><span data-stu-id="ddbf7-112">Alternate Login ID</span></span>
- <span data-ttu-id="ddbf7-113">HTTP-Proxy nicht gefunden</span><span class="sxs-lookup"><span data-stu-id="ddbf7-113">HTTP Proxy not found</span></span>

<span data-ttu-id="ddbf7-114">Behandeln von Problemen mit Geräten mithilfe des Befehls dsregcmd – [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="ddbf7-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
