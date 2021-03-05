---
title: Problem mit AAD Connect Health
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
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453293"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="0fc42-102">Problem mit AAD Connect Health</span><span class="sxs-lookup"><span data-stu-id="0fc42-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="0fc42-103">Stellen Sie sicher, dass Sie autorisiert sind, den Vorgang durchzuführen.</span><span class="sxs-lookup"><span data-stu-id="0fc42-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="0fc42-104">Globale Administratoren haben standardmäßig Zugriff.</span><span class="sxs-lookup"><span data-stu-id="0fc42-104">Global Admins have access by default.</span></span> <span data-ttu-id="0fc42-105">Darüber hinaus können Sie die rollenbasierte [Zugriffssteuerung verwenden,](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) um die Registrierungsberechtigung an den Mitwirkenden zu delegieren.</span><span class="sxs-lookup"><span data-stu-id="0fc42-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="0fc42-106">Stellen Sie sicher, dass die erforderlichen Endpunkte aktiviert und aufgrund der Firewall nicht blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="0fc42-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="0fc42-107">Weitere Informationen finden Sie unter [Requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span><span class="sxs-lookup"><span data-stu-id="0fc42-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="0fc42-108">Die Registrierung kann fehlschlagen, da ausgehende Kommunikation von der Netzwerkschicht einer SSL-Überprüfung unterzogen wird.</span><span class="sxs-lookup"><span data-stu-id="0fc42-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="0fc42-109">Stellen Sie sicher, dass Sie die Benachrichtigungseinstellungen für Azure AD Connect Health überprüft haben.</span><span class="sxs-lookup"><span data-stu-id="0fc42-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="0fc42-110">Überprüfen Sie ihre Einstellung.</span><span class="sxs-lookup"><span data-stu-id="0fc42-110">Please review your setting.</span></span> <span data-ttu-id="0fc42-111">In [diesem Handbuch](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) erfahren Sie, wie Sie die Benachrichtigungseinstellungen für Azure AD Connect-Integritätsbenachrichtigungen konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="0fc42-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="0fc42-112">Weitere Informationen zum AAD Connect Health-Synchronisierungsbericht und zum Herunterladen finden Sie unter [Synchronisierungsbericht auf Objektebene.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)</span><span class="sxs-lookup"><span data-stu-id="0fc42-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="0fc42-113">Zur Problembehandlung bei AAD Connect Health-Warnungen folgen Sie dem Problembehandlungshandbuch für [AAD Connect](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) Integritätsdaten-Warnungen und häufig gestellte Fragen unter [Common AAD Connect Health installations questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span><span class="sxs-lookup"><span data-stu-id="0fc42-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
