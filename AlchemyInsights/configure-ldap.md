---
title: Konfigurieren von LDAP
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004394"
- "7923"
ms.openlocfilehash: b6e89bca4e924c5570123194cb26358ba2c162ce
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2021
ms.locfileid: "49876573"
---
# <a name="configure-ldap"></a><span data-ttu-id="29736-102">Konfigurieren von LDAP</span><span class="sxs-lookup"><span data-stu-id="29736-102">Configure LDAP</span></span>

<span data-ttu-id="29736-103">Gehen Sie zum Konfigurieren von LDAP wie folgt vor:</span><span class="sxs-lookup"><span data-stu-id="29736-103">To configure LDAP, do the following:</span></span>

1. <span data-ttu-id="29736-104">Überprüfen Sie die Integrität Ihrer Domäne im [Azure-Portal.](https://aka.ms/aadds-health)</span><span class="sxs-lookup"><span data-stu-id="29736-104">Check your domain’s health on the [Azure portal](https://aka.ms/aadds-health).</span></span>
1. <span data-ttu-id="29736-105">Stellen Sie sicher, dass ein gültiges Azure AD-Abonnement verfügbar ist und Azure AD Domain Services aktiviert wurde.</span><span class="sxs-lookup"><span data-stu-id="29736-105">Ensure a valid Azure AD subscription is available and Azure AD Domain Services has been enabled.</span></span>
1. <span data-ttu-id="29736-106">Das zum Aktivieren von sicherem LDAP erforderliche Zertifikat muss von einer vertrauenswürdigen öffentlichen Zertifizierungsstelle oder einem selbst signierten Zertifikat erworben werden.</span><span class="sxs-lookup"><span data-stu-id="29736-106">The certificate required to enable secure LDAP must be obtained from a trusted public certification authority or be a self-signed certificate.</span></span>
1. <span data-ttu-id="29736-107">Stellen Sie sicher, dass das Zertifikat den erforderlichen Richtlinien [entspricht.](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate)</span><span class="sxs-lookup"><span data-stu-id="29736-107">Ensure the certificate follows the required [guidelines](https://docs.microsoft.com/azure/active-directory-domain-services/active-directory-ds-admin-guide-configure-secure-ldap#requirements-for-the-secure-ldap-certificate).</span></span>

<span data-ttu-id="29736-108">**Ungültiges Zertifikat**</span><span class="sxs-lookup"><span data-stu-id="29736-108">**Invalid Certificate**</span></span>
1. <span data-ttu-id="29736-109">Führen Sie zum Erneuern eines Zertifikats die schritte zum Erstellen eines neuen Zertifikats und erneuten Ladens aus: [Konfigurieren von LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="29736-109">To renew a certificate, follow the steps to create a new certificate and reupload: [Configure LDAP](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-configure-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
1. <span data-ttu-id="29736-110">Informationen zum Beheben eines bekannten Problems mit secure LDAP alerts in Azure Active directory Domain Services finden Sie unter [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="29736-110">To resolve known issue with Secure LDAP alerts in Azure Active directory Domain Services, see [Resolve LDAP alerts](https://docs.microsoft.com/azure/active-directory-domain-services/alert-ldaps?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>
