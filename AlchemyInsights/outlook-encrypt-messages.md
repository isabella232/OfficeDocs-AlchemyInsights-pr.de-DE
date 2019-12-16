---
title: S/MIME in Outlook im Internet
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053224"
---
# <a name="encrypt-email-messages-in-outlook"></a><span data-ttu-id="dc613-102">E-Mail-Nachrichten in Outlook verschlüsseln</span><span class="sxs-lookup"><span data-stu-id="dc613-102">Encrypt email messages in Outlook</span></span>

<span data-ttu-id="dc613-103">Office 365 Nachrichtenverschlüsselung basiert auf Microsoft Azure Rights Management (Azure RMS), das Teil von Azure Information Protection ist.</span><span class="sxs-lookup"><span data-stu-id="dc613-103">Office 365 Message Encryption is built on Microsoft Azure Rights Management (Azure RMS), which is part of Azure Information Protection.</span></span> <span data-ttu-id="dc613-104">Wenn Ihr Abonnement Azure Rights Management oder Azure Information Protection umfasst, **müssen Sie keine Aktionen durchführen, um den Rights Management-Dienst manuell zu aktivieren oder zu aktivieren** .</span><span class="sxs-lookup"><span data-stu-id="dc613-104">If your subscription includes Azure Rights Management or Azure Information Protection, **you do not need to take any actions to manually enable or activate** the Rights Management Service.</span></span>

<span data-ttu-id="dc613-105">Basierend auf Kundenfeedback können wir Exchange-Nachrichtenfluss Regeln nicht mehr automatisch zum automatischen Verschlüsseln von ausgehenden e-Mails mit bestimmten Typen vertraulicher Informationen in Ihrem Mandanten standardmäßig aktivieren.</span><span class="sxs-lookup"><span data-stu-id="dc613-105">Based on customer feedback, we will no longer be enabling Exchange mail flow rules to automatically encrypt outbound email containing certain type of sensitive information in your tenant by default.</span></span> <span data-ttu-id="dc613-106">Stattdessen stellen wir detaillierte Anweisungen dazu bereit, wie Sie dies selbst tun können.</span><span class="sxs-lookup"><span data-stu-id="dc613-106">Instead, we are providing detailed instructions on how you can do so yourselves.</span></span> <span data-ttu-id="dc613-107">Weitere Informationen zum Erstellen einer Transportregel zum Verschlüsseln von vertraulichen Informationen finden Sie in [diesem Artikel](https://aka.ms/OmeEtr).</span><span class="sxs-lookup"><span data-stu-id="dc613-107">For additional details on how to create a transport rule to encrypt sensitive information, see [this article](https://aka.ms/OmeEtr).</span></span>

- <span data-ttu-id="dc613-108">Bei Verwendung von Outlook im Internet (ehemals **OWA**): Klicken Sie beim Verfassen einer e-Mail-Nachricht einfach auf in OWA **schützen** .</span><span class="sxs-lookup"><span data-stu-id="dc613-108">If using Outlook on the Web (formerly **OWA**): When composing an email message, simply click **Protect** in OWA.</span></span> <span data-ttu-id="dc613-109">Dies gilt für die Berechtigung "nicht weiterleiten".</span><span class="sxs-lookup"><span data-stu-id="dc613-109">This will apply "Do not forward" permission.</span></span> <span data-ttu-id="dc613-110">Klicken Sie auf **Berechtigung ändern** , und wählen Sie **verschlüsseln** , um die Nachricht zu verschlüsseln.</span><span class="sxs-lookup"><span data-stu-id="dc613-110">Click **Change permission** and choose **Encrypt** to only encrypt the message.</span></span>

- <span data-ttu-id="dc613-111">Wenn Sie **Outlook-Client**verwenden: zum Senden einer verschlüsselten Nachricht von Outlook 2013 oder 2016 oder Outlook 2016 für Mac wählen Sie **options** > **Berechtigungen**aus, und wählen Sie dann die benötigte Schutzoption aus.</span><span class="sxs-lookup"><span data-stu-id="dc613-111">If using **Outlook client**: To send an encrypted message from Outlook 2013 or 2016, or Outlook 2016 for Mac, select **Options** > **Permissions**, then select the protection option you need.</span></span>

- <span data-ttu-id="dc613-112">Wenn Sie alle e-Mails, die an bestimmte Empfänger oder externe Partnerorganisationen gesendet werden, **automatisch verschlüsseln** möchten, müssen Sie im Exchange Admin Center eine Nachrichtenfluss-Transportregel erstellen.</span><span class="sxs-lookup"><span data-stu-id="dc613-112">To **automatically encrypt all email** sent to certain recipients or external partner organizations, you need to create a mail flow transport rule in the Exchange Admin Center.</span></span> <span data-ttu-id="dc613-113">Ausführliche Anweisungen hierzu finden Sie in [diesem Support-Artikel](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span><span class="sxs-lookup"><span data-stu-id="dc613-113">Detailed instructions are provided in [this support article](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities).</span></span>

