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
ms.openlocfilehash: 102c8025571f840cf64091d75295acec50661df2
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36530280"
---
# <a name="dlp-not-working-as-expected"></a><span data-ttu-id="b8f57-102">DLP funktioniert nicht wie erwartet</span><span class="sxs-lookup"><span data-stu-id="b8f57-102">DLP not working as expected</span></span>

<span data-ttu-id="b8f57-103">Haben Sie Probleme mit der Verhinderung von **Datenverlust (DLP)** in Office 365 nicht wie erwartet funktioniert?</span><span class="sxs-lookup"><span data-stu-id="b8f57-103">Are you having problems with **Data Loss Prevention (DLP)** in Office 365 not working as expected?</span></span> <span data-ttu-id="b8f57-104">Wenn dies der Fall ist, stellen Sie sicher, dass Ihre **DLP-Richtlinie** ordnungsgemäß eingerichtet ist und dass Ihre Daten enthalten, wonach die **DLP-Richtlinie** bei der Auswertung sucht.</span><span class="sxs-lookup"><span data-stu-id="b8f57-104">If so, make sure that your **DLP policy** is set up correctly, and that your data contains what the **DLP policy** is looking for when it is being evaluated.</span></span>
  
 <span data-ttu-id="b8f57-105">**Einrichten von DLP**</span><span class="sxs-lookup"><span data-stu-id="b8f57-105">**Setting up DLP**</span></span>
  
<span data-ttu-id="b8f57-106">Mit DLP-Richtlinien können Sie vertrauliche Informationen in Ihrer Organisation identifizieren und schützen.</span><span class="sxs-lookup"><span data-stu-id="b8f57-106">DLP policies allows you to identify and protect sensitive information in your organization.</span></span> <span data-ttu-id="b8f57-107">Verwenden Sie die Informationen [hier](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp), um DLP-Richtlinien einzurichten.</span><span class="sxs-lookup"><span data-stu-id="b8f57-107">To setup DLP policies, use the information [here](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).</span></span>
  
 <span data-ttu-id="b8f57-108">**Wonach die DLP-Richtlinien suchen**</span><span class="sxs-lookup"><span data-stu-id="b8f57-108">**What DLP policies look for**</span></span>
  
<span data-ttu-id="b8f57-109">Bei Verwendung der **integrierten Typen für vertrauliche Informationen** im Office 365 Security and Compliance Center suchen DLP-Richtlinien nach bestimmten Mustern und Elementen, wenn diese vertraulichen Typen erkannt werden.</span><span class="sxs-lookup"><span data-stu-id="b8f57-109">When using the **built-in sensitive information types** in Office 365 Security and Compliance center, DLP policies look for specific patterns and elements when detecting these sensitive types.</span></span>
  
- <span data-ttu-id="b8f57-110">**Integrierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="b8f57-110">**Built-in Sensitive Information Types**</span></span>

    <span data-ttu-id="b8f57-111">Informationen zu den integrierten vertraulichen Typen und was eine DLP-Richtlinie sucht, wenn der vertrauliche Typ erkannt wird, finden Sie unter [was die Typen vertraulicher Informationen suchen](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="b8f57-111">For information on the built-in Sensitive types and what a DLP policy looks for when detecting the Sensitive type, see: [What the sensitive information types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="b8f57-112">**Benutzerdefinierte Typen für vertrauliche Informationen**</span><span class="sxs-lookup"><span data-stu-id="b8f57-112">**Custom Sensitive Information Types**</span></span>

    <span data-ttu-id="b8f57-113">Wenn Sie versuchen, benutzerdefinierte Typen vertraulicher Informationen zu erstellen, verwenden Sie den folgenden Artikel, um Informationen zum Erstellen eines benutzerdefinierten vertraulichen Typs zu erhalten: [Erstellen eines benutzerdefinierten Typs für vertrauliche Informationen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="b8f57-113">If you are trying to create custom sensitive information types, use the following article for information on how to create a custom sensitive type: [Create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).</span></span>

<span data-ttu-id="b8f57-114">**Testen einer DLP-Richtlinie**</span><span class="sxs-lookup"><span data-stu-id="b8f57-114">**Test a DLP policy**</span></span>

<span data-ttu-id="b8f57-115">Wenn Sie Ihre Daten mit einem integrierten oder benutzerdefinierten Typ vertraulicher Informationen testen möchten, \*\*\*\* verwenden Sie die Option Testtyp unter **Klassifikationen** > **vertrauliche Informationstypen**.</span><span class="sxs-lookup"><span data-stu-id="b8f57-115">To test your data with a built-in or custom sensitive information type, use the **Test type** option under **Classifications** > **Sensitive info types**.</span></span> <span data-ttu-id="b8f57-116">Weitere Informationen finden Sie unter [Testen benutzerdefinierter vertraulicher Informationstypen](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span><span class="sxs-lookup"><span data-stu-id="b8f57-116">For more information, see [Test custom sensitive information types](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).</span></span>

 <span data-ttu-id="b8f57-117">**Berichte**</span><span class="sxs-lookup"><span data-stu-id="b8f57-117">**Reports**</span></span>
  
- <span data-ttu-id="b8f57-118">Erhalten Sie vertrauliche Daten Einblicke mit [DLP-Berichten.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span><span class="sxs-lookup"><span data-stu-id="b8f57-118">Get sensitive data insights with [DLP Reports.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)</span></span>

- <span data-ttu-id="b8f57-119">Siehe spezifische Details des Ereignisses mit einem [Vorfall Bericht](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span><span class="sxs-lookup"><span data-stu-id="b8f57-119">See specific details of the event with an [Incident Report](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).</span></span>
