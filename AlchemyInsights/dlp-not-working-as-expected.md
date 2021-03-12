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
ms.openlocfilehash: 0f07e64c95675a4f6a0aeb6df110fe4e6a21d72f
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/10/2021
ms.locfileid: "50707809"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="3ec39-102">DLP funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="3ec39-102">DLP not working as expected</span></span>

<span data-ttu-id="3ec39-103">**Wichtig**: Während dieser beispiellosen Zeiten unternehmen wir die erforderlichen Schritte, um sicherzustellen, dass SharePoint Online und OneDrive-Dienste weiterhin in hohem Ausmaß verfügbar bleiben – Bitte besuchen Sie [SharePoint Online – Temporäre Feature-Anpassungen](https://aka.ms/ODSPAdjustments), um weitere Informationen zu erhalten.</span><span class="sxs-lookup"><span data-stu-id="3ec39-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

 <span data-ttu-id="3ec39-104">**Einrichten von DLP**</span><span class="sxs-lookup"><span data-stu-id="3ec39-104">**Setting up DLP**</span></span>

<span data-ttu-id="3ec39-105">Funktionieren Probleme mit der Verhinderung von Datenverlust **(Data Loss Prevention, DLP)** in Office 365 nicht wie erwartet?</span><span class="sxs-lookup"><span data-stu-id="3ec39-105">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="3ec39-106">Wenn ja, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, was die **DLP-Richtlinie** bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="3ec39-106">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
<span data-ttu-id="3ec39-107">Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="3ec39-107">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="3ec39-108">Verwenden Sie zum Einrichten von DLP-Richtlinien die informationen [hier](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span><span class="sxs-lookup"><span data-stu-id="3ec39-108">To setup DLP policies, use the information [here](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template).</span></span>
  
 <span data-ttu-id="3ec39-109">**Suchen nach DLP-Richtlinien**</span><span class="sxs-lookup"><span data-stu-id="3ec39-109">**What DLP policies look for**</span></span>
  
<span data-ttu-id="3ec39-110">Bei der Verwendung der **integrierten** Typen vertraulicher Informationen in den Security and Compliance Centern suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.</span><span class="sxs-lookup"><span data-stu-id="3ec39-110">When using the **built-in sensitive information types** in the Security and Compliance centers, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="3ec39-111">**Integrierte Typen vertraulicher Informationen**</span><span class="sxs-lookup"><span data-stu-id="3ec39-111">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="3ec39-112">Informationen zu den integrierten Typen "Vertraulich" und zur Suche nach einer DLP-Richtlinie beim Erkennen des Typs "Vertraulich" finden Sie unter: Was die Typen vertraulicher Informationen [suchen.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)</span><span class="sxs-lookup"><span data-stu-id="3ec39-112">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>

- <span data-ttu-id="3ec39-113">**Benutzerdefinierte Typen vertraulicher Informationen**</span><span class="sxs-lookup"><span data-stu-id="3ec39-113">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="3ec39-114">Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, finden Sie im folgenden Artikel Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs: Erstellen eines benutzerdefinierten [Vertraulichen Informationstyps](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="3ec39-114">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="3ec39-115">**Testen einer DLP-Richtlinie**</span><span class="sxs-lookup"><span data-stu-id="3ec39-115">**Test a DLP policy**</span></span>

<span data-ttu-id="3ec39-116">Um Ihre Daten mit einem integrierten oder benutzerdefinierten vertraulichen Informationstyp zu testen, verwenden Sie die Option **Testtyp** unter **Klassifizierungen** Vertrauliche  >  **Infotypen**.</span><span class="sxs-lookup"><span data-stu-id="3ec39-116">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="3ec39-117">Weitere Informationen finden Sie unter [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="3ec39-117">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="3ec39-118">**Berichte**</span><span class="sxs-lookup"><span data-stu-id="3ec39-118">**Reports**</span></span>
  
- <span data-ttu-id="3ec39-119">Erhalten Sie Einblicke in vertrauliche Daten mit [DLP-Berichten.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="3ec39-119">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="3ec39-120">Siehe spezifische Details des Ereignisses mit einem [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="3ec39-120">See specific details of the event with an [Incident Report](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).</span></span>
