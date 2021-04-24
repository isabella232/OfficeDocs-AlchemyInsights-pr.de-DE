---
title: Aufbewahrungsrichtlinien im Exchange Admin Center funktionieren nicht
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952227"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="18c6f-102">Aufbewahrungsrichtlinien im Exchange Admin Center</span><span class="sxs-lookup"><span data-stu-id="18c6f-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="18c6f-103">Wenn sie möchten, dass wir automatisierte Prüfungen für die unten genannten Einstellungen ausführen, wählen Sie die Schaltfläche "Zurück" <- oben auf dieser Seite aus, und geben Sie dann die E-Mail-Adresse des Benutzers ein, der Probleme mit Aufbewahrungsrichtlinien hat.</span><span class="sxs-lookup"><span data-stu-id="18c6f-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="18c6f-104">Wenn Sie Probleme mit Aufbewahrungsrichtlinien im Exchange Admin Center haben, die nicht auf Postfächer oder Elemente angewendet werden, die nicht in das Archivpostfach verschoben werden, überprüfen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="18c6f-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="18c6f-105">**Stammursachen:**</span><span class="sxs-lookup"><span data-stu-id="18c6f-105">**Root Causes:**</span></span>

- <span data-ttu-id="18c6f-106">**Der Assistent für verwaltete** Ordner hat das Postfach des Benutzers nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="18c6f-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="18c6f-107">Der Assistent für verwaltete Ordner versucht, jedes Postfach in Ihrer cloudbasierten Organisation einmal alle sieben Tage zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="18c6f-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="18c6f-108">**Lösung:** Führen Sie den Assistenten für verwaltete Ordner aus.</span><span class="sxs-lookup"><span data-stu-id="18c6f-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="18c6f-109">**RetentionHold** wurde **für das** Postfach aktiviert.</span><span class="sxs-lookup"><span data-stu-id="18c6f-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="18c6f-110">Wenn das Postfach in einem Aufbewahrungsspeicher platziert wurde, wird die Aufbewahrungsrichtlinie für das Postfach während dieser Zeit nicht verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="18c6f-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="18c6f-111">**Lösung:** Überprüfen Sie den Status der Aufbewahrungsaufbewahrungseinstellung und aktualisieren Sie nach Bedarf.</span><span class="sxs-lookup"><span data-stu-id="18c6f-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="18c6f-112">Weitere Informationen finden Sie unter [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span><span class="sxs-lookup"><span data-stu-id="18c6f-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="18c6f-113">**Hinweis:** Wenn ein Postfach kleiner als 10 MB ist, wird das Postfach vom Assistenten für verwaltete Ordner nicht automatisch verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="18c6f-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="18c6f-114">Weitere Informationen zu Aufbewahrungsrichtlinien im Exchange Admin Center finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="18c6f-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="18c6f-115">Aufbewahrungstags und Aufbewahrungsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="18c6f-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="18c6f-116">[Anwenden einer Aufbewahrungsrichtlinie auf Postfächer oder](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) Hinzufügen oder Entfernen [von Aufbewahrungstags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="18c6f-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="18c6f-117">Identifizieren des auf ein Postfach angewandten Aufbewahrungstyps</span><span class="sxs-lookup"><span data-stu-id="18c6f-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
