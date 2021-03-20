---
title: Problembehandlung bei einmaligem Anmelden für Azure AD-beigetretene Geräte
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898084"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="be052-102">Problembehandlung bei einmaligem Anmelden für Azure AD-beigetretene Geräte</span><span class="sxs-lookup"><span data-stu-id="be052-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="be052-103">Wenn Sie über eine lokale Active Directory (AD)-Umgebung verfügen und Ihre mit der AD-Domäne beigetretenen Computer zu Azure AD hinzufügen möchten, können Sie dies erreichen, indem Sie azure AD hybrid beitreten.</span><span class="sxs-lookup"><span data-stu-id="be052-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="be052-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span><span class="sxs-lookup"><span data-stu-id="be052-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="be052-105">Weitere Informationen finden Sie unter [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="be052-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="be052-106">**Probleme mit dem primären Aktualisierungstoken (Primary Refresh Token, PRT)**</span><span class="sxs-lookup"><span data-stu-id="be052-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="be052-107">Ein primäres Aktualisierungstoken (Primary Refresh Token, PRT) ist ein Schlüsselartefakte der Azure AD-Authentifizierung auf Windows 10-, Windows Server 2016- und höher-, iOS- und Android-Geräten.</span><span class="sxs-lookup"><span data-stu-id="be052-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="be052-108">Es handelt sich um ein JSON-Webtoken (JWT), das speziell für Tokenbroker von Microsoft first party ausgegeben wurde, um einmaliges Anmelden (Single Sign-On, SSO) für die Anwendungen zu aktivieren, die auf diesen Geräten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="be052-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="be052-109">Weitere Informationen dazu, wie ein PRT auf Windows 10-Geräten ausgegeben, verwendet und geschützt wird, finden Sie unter [Was ist ein primäres Aktualisierungstoken?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="be052-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="be052-110">**WamDefaultSet: JA und AzureADPrt: JA**</span><span class="sxs-lookup"><span data-stu-id="be052-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="be052-111">Diese Felder geben an, ob sich der Benutzer erfolgreich bei Azure AD authentifiziert hat, wenn er sich beim Gerät anmeldet.</span><span class="sxs-lookup"><span data-stu-id="be052-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="be052-112">Wenn die Werte **NO sind,** kann dies auf:</span><span class="sxs-lookup"><span data-stu-id="be052-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="be052-113">Ungültiger Speicherschlüssel im TPM, das dem Gerät bei der Registrierung zugeordnet ist (überprüfen Sie den KeySignTest während der Ausführung mit erhöhten Rechten)</span><span class="sxs-lookup"><span data-stu-id="be052-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="be052-114">Alternative Anmelde-ID</span><span class="sxs-lookup"><span data-stu-id="be052-114">Alternate Login ID</span></span>
- <span data-ttu-id="be052-115">HTTP-Proxy nicht gefunden</span><span class="sxs-lookup"><span data-stu-id="be052-115">HTTP Proxy not found</span></span>

<span data-ttu-id="be052-116">Informationen zur Problembehandlung von Geräten mithilfe des Befehls dsregcmd finden Sie unter [SSO-Status](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="be052-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
