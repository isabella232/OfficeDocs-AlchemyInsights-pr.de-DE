---
title: Geräterückschreiben
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
- "9003257"
- "8279"
ms.openlocfilehash: f1a8dba19d220e1154549507801c813f56fe5cdd
ms.sourcegitcommit: 0470a728d184ceb89d1419f7ed57166e07bb778b
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/15/2021
ms.locfileid: "50255156"
---
# <a name="device-writeback"></a><span data-ttu-id="313ec-102">Geräterückschreiben</span><span class="sxs-lookup"><span data-stu-id="313ec-102">Device Writeback</span></span>

<span data-ttu-id="313ec-103">Das Rückschreiben von Geräten wird in den folgenden Szenarien verwendet:</span><span class="sxs-lookup"><span data-stu-id="313ec-103">Device Writeback is used in the following scenarios:</span></span>

- <span data-ttu-id="313ec-104">Aktivieren [von Windows Hello for Business mithilfe der Hybridbereitstellung mit Zertifikatvertrauensstellung](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span><span class="sxs-lookup"><span data-stu-id="313ec-104">Enable [Windows Hello for Business using hybrid certificate trust deployment](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-cert-trust-prereqs#device-registration)</span></span>
- <span data-ttu-id="313ec-105">Aktivieren des bedingten Zugriffs auf Basis von Geräten für ADFS (2012 R2 oder höher) geschützte Anwendungen (Vertrauensstellungen der vertrauenden Partei)</span><span class="sxs-lookup"><span data-stu-id="313ec-105">Enable Conditional Access based on devices to ADFS (2012 R2 or higher) protected applications (relying party trusts)</span></span>

    > [!NOTE]
    > <span data-ttu-id="313ec-106">Für das Rückschreiben von Geräten ist ein Abonnement für Azure AD Premium erforderlich.</span><span class="sxs-lookup"><span data-stu-id="313ec-106">A subscription to Azure AD Premium is required for device writeback.</span></span>

<span data-ttu-id="313ec-107">Dies bietet zusätzliche Sicherheit und Sicherheit, dass der Zugriff auf Anwendungen nur vertrauenswürdigen Geräten gewährt wird.</span><span class="sxs-lookup"><span data-stu-id="313ec-107">This provides additional security and assurance that access to applications is granted only to trusted devices.</span></span> <span data-ttu-id="313ec-108">Weitere Informationen zum bedingten Zugriff finden Sie unter ["Verwalten](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) von Risiken mit bedingten Zugriff" und einrichten des lokalen bedingten Zugriffs mithilfe der [Azure Active Directory-Geräteregistrierung.](https://docs.microsoft.com/azure/active-directory/devices/overview)</span><span class="sxs-lookup"><span data-stu-id="313ec-108">For more information on Conditional Access, see [Managing Risk with Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/overview) and [Setting up On-premises Conditional Access using Azure Active Directory Device Registration](https://docs.microsoft.com/azure/active-directory/devices/overview).</span></span>

<span data-ttu-id="313ec-109">Weitere Informationen zum Aktivieren des Geräterückschreibens für Geräte finden Sie unter ["Geräterückschreiben aktivieren".](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback)</span><span class="sxs-lookup"><span data-stu-id="313ec-109">For more information on Enabling Device Writeback for Devices, see [Enable Device Writeback](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-device-writeback).</span></span>
