---
title: Behandeln von Problemen bei der Azure AD Hybrid-Einbindung
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401906"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="ec6c6-102">Behandeln von Problemen bei der Azure AD Hybrid-Einbindung</span><span class="sxs-lookup"><span data-stu-id="ec6c6-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="ec6c6-103">Es wird dringend empfohlen, dass ein Gerät unter dem Systemkonto mithilfe des [Skripts zum Test der Geräteregistrierungskonnektivität](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) auf Endpunkte der Geräteregistrierung zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="ec6c6-104">Wenn Sie Geräteregistrierungen zum ersten Mal einrichten, lesen Sie unbedingt EI[nführung zur Geräteverwaltung in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), um zu erfahren, wie Sie Azure AD die Steuerung von Geräten anvertrauen.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="ec6c6-105">Wenn Sie Geräte direkt in Azure AD registrieren und für Intune registrieren, stellen Sie zuerst sicher, dass Sie [Intune konfiguriert haben](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) und die [-Lizenzierung](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) zur Verfügung haben.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="ec6c6-106">Stellen Sie sicher, dass Sie autorisiert sind, Vorgänge in Azure AD und lokalem AD durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="ec6c6-107">Nur ein globaler Administrator in Azure AD kann Einstellungen für Geräteregistrierungen verwalten.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="ec6c6-108">Wenn Sie außerdem automatische Registrierungen in Ihrem lokalen Active Directory einrichten, müssen Sie außerdem Administrator von Active Directory und (sofern zutreffend) AD FS sein.</span><span class="sxs-lookup"><span data-stu-id="ec6c6-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="ec6c6-109">Weitere Details zum Beheben potenzieller Probleme mit der Hybridverknüpfung finden Sie unter [Problembehandlung bei der Hybridverknüpfung](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) zum Einrichten von mit Azure AD verknüpften Hybridgeräten und zum Verwalten von Geräten mithilfe des Azure AD-Portals finden Sie unter [Einrichten von mit Azure AD verknüpften Hybridgeräten (lokal domänenverknüpften)](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) und [Verwalten von Geräten mithilfe des Azure-Portals](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="ec6c6-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="ec6c6-110">Informationen zum Beheben von häufig auftretenden Problemen bei der Azure AD Hybrid-Einbindung finden Sie unter [Häufig gestellte Fragen zu Azure AD Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="ec6c6-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
