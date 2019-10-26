---
title: Deaktivieren externer Gruppen
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: b2328ea85d3ff6ec722cc56d8a46395d8438f79c
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 10/25/2019
ms.locfileid: "36739492"
---
# <a name="how-to-disable-external-groups"></a><span data-ttu-id="fdc96-102">Deaktivieren externer Gruppen</span><span class="sxs-lookup"><span data-stu-id="fdc96-102">How to disable External Groups</span></span>

<span data-ttu-id="fdc96-103">"Jammern" externes Messaging wendet Exchange-Transport Regeln (ETRs) an, eine Gruppe proaktiver Steuerelemente, um zu verhindern, dass Unternehmensinformationen freigegeben werden.</span><span class="sxs-lookup"><span data-stu-id="fdc96-103">Yammer external messaging applies Exchange Transport Rules (ETRs), a set of proactive controls to prevent company information from being shared.</span></span> <span data-ttu-id="fdc96-104">Um Benutzer daran zu hindern, externe Gruppen zu erstellen, müssen Sie eine Exchange-Transportregel (ETR) konfigurieren und dann jammern konfigurieren, damit die Exchange-Transportregel zum Blockieren von externem Messaging verwendet wird.</span><span class="sxs-lookup"><span data-stu-id="fdc96-104">In order to restrict users from creating external groups, you need to configure an Exchange transport rule (ETR), and then configure Yammer to use the Exchange Transport rule to block external messaging.</span></span>
  
<span data-ttu-id="fdc96-105">Nachdem Sie eine Regel in Exchange Online Admin Center erstellt haben, führen Sie die folgenden Schritte aus, um ETR so festzulegen, dass Sie in "jammern" angewendet wird:</span><span class="sxs-lookup"><span data-stu-id="fdc96-105">Once you have created a rule in Exchange Online admin center, follow these steps to set ETR to apply in Yammer:</span></span>
  
- <span data-ttu-id="fdc96-106">Melden Sie sich bei jammern als überprüfter Administrator an, und wechseln Sie im **Admin Center**zu C- **Inhalts \> -und Sicherheits Sicherheitseinstellungen.**</span><span class="sxs-lookup"><span data-stu-id="fdc96-106">Log on to Yammer as a verified admin, and in the **Yammer admin center**, go to C **Content and Security \> Security Settings.**</span></span>

- <span data-ttu-id="fdc96-107">Wählen Sie unter **externes Messaging** **die Option Erzwingen der Exchange Online Exchange-Transport Regeln (ETRs) in jammern aus.**</span><span class="sxs-lookup"><span data-stu-id="fdc96-107">Under **External Messaging**, select **Enforce your Exchange Online Exchange Transport Rules (ETRs) in Yammer.**</span></span>

- <span data-ttu-id="fdc96-108">Wählen Sie **Speichern** aus.</span><span class="sxs-lookup"><span data-stu-id="fdc96-108">Choose **Save**.</span></span>

<span data-ttu-id="fdc96-109">Weitere Informationen finden Sie unter [Disable External Messaging in a jammern Network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span><span class="sxs-lookup"><span data-stu-id="fdc96-109">For more information, see [Disable external messaging in a Yammer network](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging).</span></span>
  