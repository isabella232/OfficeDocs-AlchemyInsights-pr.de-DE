---
title: DLP funktioniert nicht wie erwartet
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 0ed893420b5813d5d18639c2c226c12f0306a13f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679692"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="d771a-102">DLP funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="d771a-102">DLP not working as expected</span></span>

<span data-ttu-id="d771a-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="d771a-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="d771a-104">**Einrichten von DLP**</span><span class="sxs-lookup"><span data-stu-id="d771a-104">**Setting up DLP**</span></span>

<span data-ttu-id="d771a-105">Haben Sie Probleme mit der **Verhinderung von Datenverlust (DLP)** in Office 365 nicht wie erwartet funktioniert?</span><span class="sxs-lookup"><span data-stu-id="d771a-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="d771a-106">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="d771a-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="d771a-107">Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="d771a-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="d771a-108">Verwenden Sie die Informationen [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp), um DLP-Richtlinien einzurichten.</span><span class="sxs-lookup"><span data-stu-id="d771a-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="d771a-109">**Wonach die DLP-Richtlinien suchen**</span><span class="sxs-lookup"><span data-stu-id="d771a-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="d771a-110">Bei Verwendung der **integrierten Typen vertraulicher Informationen** im Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.</span><span class="sxs-lookup"><span data-stu-id="d771a-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="d771a-111">**Integrierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="d771a-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="d771a-112">Informationen zu den integrierten vertraulichen Typen und was eine DLP-Richtlinie sucht, wenn der vertrauliche Typ erkannt wird, finden Sie unter [was die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="d771a-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="d771a-113">**Benutzerdefinierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="d771a-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="d771a-114">Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="d771a-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="d771a-115">**Testen einer DLP-Richtlinie**</span><span class="sxs-lookup"><span data-stu-id="d771a-115">**Test a DLP policy**</span></span>

<span data-ttu-id="d771a-116">Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten Typ vertraulicher Informationen testen möchten, verwenden Sie die Option **Testtyp** unter **Klassifikationen**  >  **vertrauliche Informationstypen**.</span><span class="sxs-lookup"><span data-stu-id="d771a-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="d771a-117">Weitere Informationen finden Sie unter [Testen benutzerdefinierter vertraulicher Informationstypen](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="d771a-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="d771a-118">**Berichte**</span><span class="sxs-lookup"><span data-stu-id="d771a-118">**Reports**</span></span>
  
- <span data-ttu-id="d771a-119">Erhalten Sie vertrauliche Daten Einblicke mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="d771a-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="d771a-120">Siehe spezifische Details des Ereignisses mit einem [Vorfall Bericht](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="d771a-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
