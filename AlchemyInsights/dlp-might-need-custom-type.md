---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507513"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="bccec-102">DLP benötigt möglicherweise einen benutzerdefinierten Typ</span><span class="sxs-lookup"><span data-stu-id="bccec-102">DLP might need a custom type</span></span>

<span data-ttu-id="bccec-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="bccec-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="bccec-104">**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp.**</span><span class="sxs-lookup"><span data-stu-id="bccec-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="bccec-105">Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="bccec-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="bccec-106">In einigen Szenarien müssen Sie möglicherweise einen eigenen **benutzerdefinierten** Typ für vertrauliche Informationen erstellen, um die Daten Ihrer Organisation zu schützen.</span><span class="sxs-lookup"><span data-stu-id="bccec-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="bccec-107">Beispielsweise kann es sein, dass Ihre Organisation Mitarbeiter-IDs oder andere Daten in einem bestimmten für Ihre org spezifischen Format identifizieren und schützen muss. Wenn dies der Fall ist, finden Sie weitere Informationen in den folgenden Artikeln.</span><span class="sxs-lookup"><span data-stu-id="bccec-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="bccec-108">**Anpassen eines benutzerdefinierten vertraulichen Informationstyps**</span><span class="sxs-lookup"><span data-stu-id="bccec-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="bccec-109">Wenn ein integrierter vertraulicher Informationstyp Ihren Anforderungen mit nur wenigen Optimierungen entspricht, können Sie [einen integrierten vertraulichen Informationstyp anpassen](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="bccec-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="bccec-110">Beispielsweise können Sie Stichwörter hinzufügen oder entfernen oder unterstützende Beweise wie ein Datum oder eine Adresse hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="bccec-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="bccec-111">**Erstellen eines benutzerdefinierten vertraulichen Informationstyps**</span><span class="sxs-lookup"><span data-stu-id="bccec-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="bccec-112">Wenn Sie jedoch einen anderen Typ vertraulicher Informationen insgesamt identifizieren und schützen müssen, können Sie [einen benutzerdefinierten Typ vertraulicher Informationen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) auf der Benutzeroberfläche des Security & Compliance Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="bccec-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="bccec-113">**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="bccec-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="bccec-114">Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie [in Security & Compliance Center PowerShell einen benutzerdefinierten Typ für vertrauliche Informationen erstellen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="bccec-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="bccec-115">Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden.</span><span class="sxs-lookup"><span data-stu-id="bccec-115">By starting with an XML file, you can use every option available.</span></span>
