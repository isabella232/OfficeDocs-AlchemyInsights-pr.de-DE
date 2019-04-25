---
title: Deaktivieren externer Gruppen
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 4d911c319c3e8e327f9b3af3ba67816e646bc468
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399590"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="1de40-102">Deaktivieren externer Gruppen</span><span class="sxs-lookup"><span data-stu-id="1de40-102">How to disable External Groups</span></span>

<span data-ttu-id="1de40-103">Jammern externe Messaging wendet Exchange-Transport Regeln (ETRs), eine Reihe proaktiver Steuerelemente an, um zu verhindern, dass Unternehmensinformationen freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="1de40-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="1de40-104">Um Benutzer daran zu hindern, externe Gruppen zu erstellen, müssen Sie eine Exchange-Transportregel (ETR) konfigurieren und dann jammern konfigurieren, dass die Exchange-Transportregel zum Blockieren von externem Messaging verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="1de40-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span> 
  
<span data-ttu-id="1de40-105">Nachdem Sie eine Regel in Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR auf Anwenden in jammern festzulegen:</span><span class="sxs-lookup"><span data-stu-id="1de40-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="1de40-106">Melden Sie sich bei jammern als verifizierter Administrator an, und wechseln Sie im **Jammer Verwaltungscenter**zu C ontent \*\* \> und Sicherheits Sicherheitseinstellungen.\*\*</span><span class="sxs-lookup"><span data-stu-id="1de40-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **ontent and Security \> Security Settings.**</span></span>
    
- <span data-ttu-id="1de40-107">Wählen Sie unter **externe Nachrichtenübermittlung** **die Option Exchange Online-Transport Regeln erzwingen (ETRs) in jammern aus.**</span><span class="sxs-lookup"><span data-stu-id="1de40-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>
    
- <span data-ttu-id="1de40-108">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="1de40-108">Choose **Save**.</span></span> 
    
<span data-ttu-id="1de40-109">Weitere Informationen finden Sie unter [Steuerelement für externe Nachrichten in einem Jammer-Netzwerk mit Exchange-Transport Regeln](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9) .</span><span class="sxs-lookup"><span data-stu-id="1de40-109">For more information, see [Control external messaging in a Yammer network with Exchange Transport rules](https://support.office.com/article/Control-external-messaging-in-a-Yammer-network-with-Exchange-Transport-Rules-f8fd6403-c8f3-4307-9230-65304d6000d9)</span></span>
  

