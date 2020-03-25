---
title: DLP benötigt möglicherweise einen benutzerdefinierten Typ
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932657"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="4eaf7-102">DLP benötigt möglicherweise einen benutzerdefinierten Typ</span><span class="sxs-lookup"><span data-stu-id="4eaf7-102">DLP might need a custom type</span></span>

<span data-ttu-id="4eaf7-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4eaf7-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4eaf7-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4eaf7-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4eaf7-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4eaf7-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4eaf7-109">**DLP erfordert möglicherweise einen benutzerdefinierten Informationstyp.**</span><span class="sxs-lookup"><span data-stu-id="4eaf7-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="4eaf7-110">Mit einer Richtlinie zur Verhinderung von Datenverlust (Data Loss Prevention, DLP) können Sie vertrauliche Daten in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="4eaf7-111">In einigen Szenarien müssen Sie möglicherweise einen eigenen **benutzerdefinierten** Typ für vertrauliche Informationen erstellen, um die Daten Ihrer Organisation zu schützen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="4eaf7-112">Beispielsweise kann es sein, dass Ihre Organisation Mitarbeiter-IDs oder andere Daten in einem bestimmten für Ihre org spezifischen Format identifizieren und schützen muss. Wenn dies der Fall ist, finden Sie weitere Informationen in den folgenden Artikeln.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="4eaf7-113">**Anpassen eines benutzerdefinierten vertraulichen Informationstyps**</span><span class="sxs-lookup"><span data-stu-id="4eaf7-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="4eaf7-114">Wenn ein integrierter vertraulicher Informationstyp Ihren Anforderungen mit nur wenigen Optimierungen entspricht, können Sie [einen integrierten vertraulichen Informationstyp anpassen](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="4eaf7-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="4eaf7-115">Beispielsweise können Sie Stichwörter hinzufügen oder entfernen oder unterstützende Beweise wie ein Datum oder eine Adresse hinzufügen oder entfernen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="4eaf7-116">**Erstellen eines benutzerdefinierten vertraulichen Informationstyps**</span><span class="sxs-lookup"><span data-stu-id="4eaf7-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="4eaf7-117">Wenn Sie jedoch einen anderen Typ vertraulicher Informationen insgesamt identifizieren und schützen müssen, können Sie [einen benutzerdefinierten Typ vertraulicher Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) auf der Benutzeroberfläche des Security & Compliance Center erstellen.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="4eaf7-118">**Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen in Security & Compliance Center PowerShell**</span><span class="sxs-lookup"><span data-stu-id="4eaf7-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="4eaf7-119">Wenn die Benutzeroberfläche nicht alle benötigten Optionen bereitstellt, können Sie [in Security & Compliance Center PowerShell einen benutzerdefinierten Typ für vertrauliche Informationen erstellen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="4eaf7-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="4eaf7-120">Wenn Sie mit einer XML-Datei beginnen, können Sie jede verfügbare Option verwenden.</span><span class="sxs-lookup"><span data-stu-id="4eaf7-120">By starting with an XML file, you can use every option available.</span></span>
