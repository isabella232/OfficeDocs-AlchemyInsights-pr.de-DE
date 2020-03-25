---
title: DLP funktioniert nicht wie erwartet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932621"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="24aef-102">DLP funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="24aef-102">DLP not working as expected</span></span>

<span data-ttu-id="24aef-103">**Wichtig**: viele SharePoint Online-und OneDrive-Kunden führen geschäftskritische Anwendungen für den Dienst aus, der im Hintergrund ausgeführt wird.</span><span class="sxs-lookup"><span data-stu-id="24aef-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="24aef-104">Dazu gehören Inhaltsmigration, Verhinderung von Datenverlusten (Data Loss Prevention, DLP) und Sicherungslösungen.</span><span class="sxs-lookup"><span data-stu-id="24aef-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="24aef-105">In diesen noch nie dagewesenen Zeiten machen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online- und OneDrive-Dienste für Ihre Benutzer, die von dem Dienst in Remotearbeitsszenarien mehr denn je abhängig sind, weiterhin hochgradig verfügbar und zuverlässig sind.</span><span class="sxs-lookup"><span data-stu-id="24aef-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="24aef-106">Zur Unterstützung dieses Ziels haben wir strengere Drosselungsgrenzen für Hintergrundanwendungen (Migration, DLP und Sicherungslösungen) während der Tageszeit unter der Woche eingeführt.</span><span class="sxs-lookup"><span data-stu-id="24aef-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="24aef-107">Sie sollten davon ausgehen, dass diese Apps in diesen Zeiten einen sehr begrenzten Durchsatz erreichen.</span><span class="sxs-lookup"><span data-stu-id="24aef-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="24aef-108">Während der Abendstunden und an Wochenenden wird der Dienst für die Region jedoch in der Lage sein, ein erheblich höheres Volumen an Anforderungen von Hintergrundanwendungen zu verarbeiten.</span><span class="sxs-lookup"><span data-stu-id="24aef-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

 <span data-ttu-id="24aef-109">**Einrichten von DLP**</span><span class="sxs-lookup"><span data-stu-id="24aef-109">**Setting up DLP**</span></span>

<span data-ttu-id="24aef-110">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** in Office 365 nicht wie erwartet funktioniert?</span><span class="sxs-lookup"><span data-stu-id="24aef-110">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="24aef-111">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="24aef-111">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="24aef-112">Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="24aef-112">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="24aef-113">Verwenden Sie die Informationen [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp), um DLP-Richtlinien einzurichten.</span><span class="sxs-lookup"><span data-stu-id="24aef-113">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="24aef-114">**Wonach die DLP-Richtlinien suchen**</span><span class="sxs-lookup"><span data-stu-id="24aef-114">**What DLP policies look for**</span></span>
  
<span data-ttu-id="24aef-115">Bei Verwendung der **integrierten Typen für vertrauliche Informationen** im Office 365 Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.</span><span class="sxs-lookup"><span data-stu-id="24aef-115">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="24aef-116">**Integrierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="24aef-116">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="24aef-117">Informationen zu den integrierten vertraulichen Typen und was eine DLP-Richtlinie sucht, wenn der vertrauliche Typ erkannt wird, finden Sie unter [was die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="24aef-117">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="24aef-118">**Benutzerdefinierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="24aef-118">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="24aef-119">Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="24aef-119">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="24aef-120">**Testen einer DLP-Richtlinie**</span><span class="sxs-lookup"><span data-stu-id="24aef-120">**Test a DLP policy**</span></span>

<span data-ttu-id="24aef-121">Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten Typ vertraulicher Informationen testen möchten, verwenden Sie die Option **Testtyp** unter **Klassifikationen** > **vertrauliche Informationstypen**.</span><span class="sxs-lookup"><span data-stu-id="24aef-121">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="24aef-122">Weitere Informationen finden Sie unter [Testen benutzerdefinierter vertraulicher Informationstypen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="24aef-122">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="24aef-123">**Berichte**</span><span class="sxs-lookup"><span data-stu-id="24aef-123">**Reports**</span></span>
  
- <span data-ttu-id="24aef-124">Erhalten Sie vertrauliche Daten Einblicke mit [DLP-Berichten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="24aef-124">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="24aef-125">Siehe spezifische Details des Ereignisses mit einem [Vorfall Bericht](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="24aef-125">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
