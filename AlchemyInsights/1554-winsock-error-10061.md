---
title: 1554 10061 Winsock-Fehler
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 9331a6c2b6e92a66fb97daf7dc5655ec320cba0f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29903096"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="b429d-102">Winsock-Fehler 10061</span><span class="sxs-lookup"><span data-stu-id="b429d-102">Winsock error 10061</span></span>

<span data-ttu-id="b429d-p101">Dieser Fehlercode bedeutet, dass einen TCP-Socket (Verbindung) mit den Zielhost ein Office 365 hergestellt werden konnte nicht. Höchstwahrscheinlich für diesen Fehler ist ein Problem mit der Konfiguration Ihrer Firewall. Um das Problem zu beheben, überprüfen Sie diese Einstellungen:</span><span class="sxs-lookup"><span data-stu-id="b429d-p101">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host. The most likely cause of this error is a problem with your firewall configuration. To fix the problem, check these settings:</span></span>
  
- <span data-ttu-id="b429d-106">Überprüfen Sie die Konfiguration Ihrer Firewall mit den Informationen in [Office 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="b429d-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>
    
- <span data-ttu-id="b429d-107">Wenn der Fehler bestimmte Exchange Online Protection (EOP) ist, sollten haben Sie bereits auf eine Änderung der [Exchange Online Protection-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)benachrichtigt.</span><span class="sxs-lookup"><span data-stu-id="b429d-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>
    
- <span data-ttu-id="b429d-108">Stellen Sie sicher, dass Ihr Internetdienstanbieter (ISP) den Port nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="b429d-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>
    
- <span data-ttu-id="b429d-109">Vergewissern Sie sich smart Host und Ziel-servereinstellungen in die Connectors.</span><span class="sxs-lookup"><span data-stu-id="b429d-109">Verify the smart host and target server settings in your connectors.</span></span>
    
<span data-ttu-id="b429d-110">Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="b429d-110">Note that Office 365 doesn't block  *incoming*  connections in this manner.</span></span> 
  

