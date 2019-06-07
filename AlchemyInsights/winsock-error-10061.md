---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 3fa3b2f2e10d3ebe480861e1f2d7ecaa262afe14
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757090"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="f06b7-102">Winsock-Fehler 10061</span><span class="sxs-lookup"><span data-stu-id="f06b7-102">Winsock error 10061</span></span>

<span data-ttu-id="f06b7-103">Dieser Fehlercode bedeutet, dass Office 365 keinen TCP-Socket (Connection) mit dem Ziel Host einrichten konnten.</span><span class="sxs-lookup"><span data-stu-id="f06b7-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="f06b7-104">Die wahrscheinlichste Ursache dieses Fehlers ist ein Problem mit der Konfiguration Ihrer Firewall.</span><span class="sxs-lookup"><span data-stu-id="f06b7-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="f06b7-105">Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:</span><span class="sxs-lookup"><span data-stu-id="f06b7-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="f06b7-106">Überprüfen der Firewall-Konfiguration mit den Informationen in [Office 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="f06b7-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="f06b7-107">Wenn der Fehler spezifisch für Exchange Online Protection (EoP) ist, sollten Sie zuvor eine Änderung an den [IP-Adressen des Exchange Online Schutzes](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.</span><span class="sxs-lookup"><span data-stu-id="f06b7-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="f06b7-108">Stellen Sie sicher, dass der Internetdienstanbieter den Port nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="f06b7-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="f06b7-109">Überprüfen Sie die Einstellungen für Smart Host und Zielserver in ihren Connectors.</span><span class="sxs-lookup"><span data-stu-id="f06b7-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="f06b7-110">Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="f06b7-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
