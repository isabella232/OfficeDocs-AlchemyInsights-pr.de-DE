---
title: 1554 Winsock-Fehler 10061
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 12/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1554
ms.assetid: caecfa19-86c9-4aa4-9c83-b8a974ce60b9
ms.openlocfilehash: 7651effc43cb0c4bc2fbbe5349bb72303943f493
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859139"
---
# <a name="winsock-error-10061"></a><span data-ttu-id="c16de-102">Winsock-Fehler 10061</span><span class="sxs-lookup"><span data-stu-id="c16de-102">Winsock error 10061</span></span>

<span data-ttu-id="c16de-103">Dieser Fehlercode besagt, dass Office 365 keinen TCP-Socket (Verbindung) mit dem Zielhost herstellen konnte.</span><span class="sxs-lookup"><span data-stu-id="c16de-103">This error code means that Office 365 couldn't establish a TCP socket (connection) with the target host.</span></span> <span data-ttu-id="c16de-104">Die wahrscheinlichste Ursache für diesen Fehler ist ein Problem mit der Konfiguration Ihrer Firewall.</span><span class="sxs-lookup"><span data-stu-id="c16de-104">The most likely cause of this error is a problem with your firewall configuration.</span></span> <span data-ttu-id="c16de-105">Um das Problem zu beheben, überprüfen Sie die folgenden Einstellungen:</span><span class="sxs-lookup"><span data-stu-id="c16de-105">To fix the problem, check these settings:</span></span>

- <span data-ttu-id="c16de-106">Überprüfen der Firewall-Konfiguration mit den Informationen in [Office 365-URLs und IP-Adressbereichen](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span><span class="sxs-lookup"><span data-stu-id="c16de-106">Verify your firewall configuration with the information in [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)</span></span>

- <span data-ttu-id="c16de-107">Wenn der Fehler spezifisch für Exchange Online Protection (EOP) ist, sollten Sie zuvor eine Änderung an den [Exchange Online Protection-IP-Adressen](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses)mitgeteilt haben.</span><span class="sxs-lookup"><span data-stu-id="c16de-107">If the error is specific to Exchange Online Protection (EOP), you should have been previously notified to a change to the [Exchange Online Protection IP addresses](https://docs.microsoft.com/office365/SecurityCompliance/eop/exchange-online-protection-ip-addresses).</span></span>

- <span data-ttu-id="c16de-108">Stellen Sie sicher, dass der InternetdienstAnbieter den Anschluss nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="c16de-108">Verify that your Internet Service Provider (ISP) isn't blocking the port.</span></span>

- <span data-ttu-id="c16de-109">Überprüfen Sie die Einstellungen für Smarthost und Zielserver in ihren Connectors.</span><span class="sxs-lookup"><span data-stu-id="c16de-109">Verify the smart host and target server settings in your connectors.</span></span>

<span data-ttu-id="c16de-110">Beachten Sie, dass Office 365 *eingehende* Verbindungen auf diese Weise nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="c16de-110">Note that Office 365 doesn't block *incoming* connections in this manner.</span></span>
