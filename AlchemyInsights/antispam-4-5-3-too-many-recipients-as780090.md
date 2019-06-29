---
title: 1049 Antispam 4.5.3 zu viele Empfänger (AS780090)
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 9/28/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1049"
- "3100024"
ms.assetid: fa3d4be9-c90a-4926-9754-4b708b038bf6
ms.openlocfilehash: 841691026560692942dfd78442e91f2b57fcbb63
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35357028"
---
# <a name="453-too-many-recipients-as780090"></a><span data-ttu-id="32c23-102">4.5.3 zu viele Empfänger (AS780090)</span><span class="sxs-lookup"><span data-stu-id="32c23-102">4.5.3 Too many recipients (AS780090)</span></span>

<span data-ttu-id="32c23-103">Dieser Fehler tritt auf, wenn der e-Mail-Datenverkehr von der Quell-IP-Adresse den Grenzwert überschreitet, der auf der Reputation (oder mangelnden Reputation) der Quell-IP-Adresse basiert.</span><span class="sxs-lookup"><span data-stu-id="32c23-103">This error occurs when the volume of email traffic from the source IP address exceeds the limit based on the reputation (or lack of reputation) of source IP address.</span></span>

<span data-ttu-id="32c23-104">Das Blockieren von e-Mails von der Quell-IP-Adresse läuft innerhalb einer Stunde ab.</span><span class="sxs-lookup"><span data-stu-id="32c23-104">Blocking email from the source IP address will expire within an hour.</span></span> <span data-ttu-id="32c23-105">Wenn es sich bei der Quell-IP-Adresse um einen lokalen e-Mail-Server handelt, der Ihnen gehört, überprüfen Sie die Konfiguration des Nachrichtenfluss-Konnektors.</span><span class="sxs-lookup"><span data-stu-id="32c23-105">If the source IP address is an on-premises email server that belongs to you, verify the configuration of the mail flow connector.</span></span> <span data-ttu-id="32c23-106">Wenn das Verhalten länger als eine Stunde dauert, wenden Sie sich an den Support, um eine Ausnahme für die Quell-IP-Adresse anzufordern.</span><span class="sxs-lookup"><span data-stu-id="32c23-106">If the behavior continues for more than an hour, contact support to request an exception for the source IP address.</span></span>
