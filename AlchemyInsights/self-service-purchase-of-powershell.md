---
title: Self-Service-Kauf von PowerShell
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797720"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="89404-102">Self-Service-Kauf von PowerShell</span><span class="sxs-lookup"><span data-stu-id="89404-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="89404-103">Zum Verwenden des MS Commerce PowerShell-Moduls müssen Sie es auf einem Windows 10-Gerät mit TLS 1.2 installieren (lokale Administratorberechtigungen erforderlich).</span><span class="sxs-lookup"><span data-stu-id="89404-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="89404-104">Importieren und Herstellen einer Verbindung mit dem MS Commerce-Modul.</span><span class="sxs-lookup"><span data-stu-id="89404-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="89404-105">Wenn Sie zur Anmeldung aufgefordert werden, müssen Sie anmeldeinformationen für globale Oder Abrechnungsadministratoren verwenden.</span><span class="sxs-lookup"><span data-stu-id="89404-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="89404-106">Wenn Sie nicht über TLS 1.2 verfügen, wird möglicherweise der folgende Fehler angezeigt, wenn Sie versuchen, die Richtlinie zu erhalten oder zu aktualisieren:</span><span class="sxs-lookup"><span data-stu-id="89404-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="89404-107">*ErrorMessage – Die zugrunde liegende Verbindung wurde geschlossen: Bei* einem Senden ist ein unerwarteter Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="89404-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



