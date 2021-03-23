---
title: Diagnose für verschiedene Probleme beim Zugriff auf Ports
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9035"
- "9005220"
ms.openlocfilehash: 3673067cad7ac55f3820422dc2ec09942c393149
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897615"
---
# <a name="diagnostics-for-different-ports-access-issues"></a><span data-ttu-id="1737c-102">Diagnose für verschiedene Probleme beim Zugriff auf Ports</span><span class="sxs-lookup"><span data-stu-id="1737c-102">Diagnostics for different ports access issues</span></span>

<span data-ttu-id="1737c-103">Führen Sie die folgenden Schritte aus, um die verschiedenen Probleme beim Portzugriff zu beheben:</span><span class="sxs-lookup"><span data-stu-id="1737c-103">To resolve the different port access issues, perform the following steps:</span></span>

1. <span data-ttu-id="1737c-104">Beenden/Freigabe der virtuellen Maschine (VM) vom Portal aus, starten Sie die VM neu und testen Sie diese erneut.</span><span class="sxs-lookup"><span data-stu-id="1737c-104">Stop/deallocate the virtual machine (VM) from the portal, restart the VM, and test again.</span></span> 
2. <span data-ttu-id="1737c-105">Überprüfen Sie die Netzwerkeinstellungen Ihrer VM, um festzustellen, ob Network Security Groups (NSGs) den Datenverkehr blockieren.</span><span class="sxs-lookup"><span data-stu-id="1737c-105">Check your VM's network settings to determine if you have Network Security Groups (NSGs) blocking traffic.</span></span> <span data-ttu-id="1737c-106">Sie können auch das [IP-Flussüberprüfungstool von Network Watcher](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) verwenden, um zu überprüfen, ob NSGs den Datenverkehr blockieren, benutzerdefinierte Routen (User Defined Routes, UDRs), die Ihren Datenverkehr zurück zu lokalen ('Standardroute' 0.0.0.0/0) oder zu einer Netzwerk-Anwendung umleiten.</span><span class="sxs-lookup"><span data-stu-id="1737c-106">You can also use [Network Watcher's IP flow verify tool](https://docs.microsoft.com/azure/network-watcher/network-watcher-ip-flow-verify-overview?WT.mc_id=Portal-Microsoft_Azure_Support) to check for NSGs blocking traffic, User-Defined Routes (UDRs) rerouting your traffic back to on-premises ('Default Route' 0.0.0.0/0), or to a network appliance.</span></span>
<span data-ttu-id="1737c-107">Wenn nach dem Ausführen der obigen Schritte weiterhin Probleme auftreten, geben Sie den VM-Namen und den TCP-Port an, an den Sie E-Mails zur weiteren Diagnose senden möchten.</span><span class="sxs-lookup"><span data-stu-id="1737c-107">If you still experience issues after trying the steps above, please provide the VM name and the TCP port you are attempting to send mail on for further diagnosis.</span></span>

<span data-ttu-id="1737c-108">**Empfohlene Dokumente**</span><span class="sxs-lookup"><span data-stu-id="1737c-108">**Recommended Documents**</span></span>

[<span data-ttu-id="1737c-109">Einschränkungen und Empfehlungen für das Senden ausgehender E-Mails über Port 25</span><span class="sxs-lookup"><span data-stu-id="1737c-109">Limitations and recommendations for sending outbound email over port 25</span></span>](https://docs.microsoft.com/azure/virtual-network/troubleshoot-outbound-smtp-connectivity)