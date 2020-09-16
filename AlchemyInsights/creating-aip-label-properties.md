---
title: Erstellen von AIP-Bezeichnungsrichtlinien
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732174"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="16758-102">Erstellen von AIP-Bezeichnungsrichtlinien</span><span class="sxs-lookup"><span data-stu-id="16758-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="16758-103">AIP-Bezeichnungen (Azure Information Protection) können mit dem vollständigen Datenbereich verwendet werden, den eine Organisation normalerweise erstellt, und speichert von der niedrigsten Klassifizierung der personenbezogenen Daten bis hin zur höchsten Klassifizierung streng vertraulicher Daten.</span><span class="sxs-lookup"><span data-stu-id="16758-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="16758-104">Azure Information Protection-Richtlinien gelten für den Azure Information Protection (AIP) Classic-Client und nicht für den  [AIP Unified Labeling-Client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="16758-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="16758-105">Sie können mehrere Elemente in einer AIP-Richtlinie konfigurieren, einschließlich Optionen wie:</span><span class="sxs-lookup"><span data-stu-id="16758-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="16758-106">Option für das Label lässt Administratoren oder Benutzer klassifizieren und schützen (optional) Dokumente und e-Mails</span><span class="sxs-lookup"><span data-stu-id="16758-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="16758-107">Option zum Erzwingen der Klassifizierung, wenn Benutzer Dokumente speichern und e-Mails senden</span><span class="sxs-lookup"><span data-stu-id="16758-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="16758-108">Option zum automatischen beschriften einer e-Mail-Nachricht basierend auf ihren Anlagen.</span><span class="sxs-lookup"><span data-stu-id="16758-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="16758-109">Option zum Steuern, ob die Informationsschutz Leiste in Office-Anwendungen angezeigt wird</span><span class="sxs-lookup"><span data-stu-id="16758-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="16758-110">Weitere Optionen und Informationen zu Azure Information Protection-Richtlinien finden Sie unter: [Overview of the Azure Information Protection Policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="16758-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="16758-111">Weitere hilfreiche Ressourcen zu AIP-Richtlinien finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="16758-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="16758-112">Tutorial: Konfigurieren von Azure Information Protection-Richtlinieneinstellungen und Erstellen einer neuen Bezeichnung</span><span class="sxs-lookup"><span data-stu-id="16758-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="16758-113">Konfigurieren der Azure Information Protection-Richtlinie</span><span class="sxs-lookup"><span data-stu-id="16758-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="16758-114">Erstellen und Konfigurieren von Vertraulichkeitsbezeichnungen und deren Richtlinien</span><span class="sxs-lookup"><span data-stu-id="16758-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="16758-115">Kurzanleitungen für häufige Szenarios, in denen Azure Information Protection verwendet wird</span><span class="sxs-lookup"><span data-stu-id="16758-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="16758-116">Nachschlagen in der Azure Information Protection-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="16758-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="16758-117">Anforderungen für Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="16758-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="16758-118">Schnellstart-Tutorial für Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="16758-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="16758-119">Azure Information Protection Client herunterladen</span><span class="sxs-lookup"><span data-stu-id="16758-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)