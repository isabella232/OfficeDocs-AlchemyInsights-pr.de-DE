---
title: 'AIP: Richtlinien zeigen nicht das erwartete Verhalten'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002266"
- "4780"
ms.openlocfilehash: 7baa010cc0b18b5d2a295623639fabf2bc5f88ec
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821626"
---
# <a name="aip-policies-not-behaving-as-expected"></a><span data-ttu-id="70499-102">AIP: Richtlinien zeigen nicht das erwartete Verhalten</span><span class="sxs-lookup"><span data-stu-id="70499-102">AIP: Policies not behaving as expected</span></span>

<span data-ttu-id="70499-103">Azure Information Protection: Zeigen Richtlinien nicht das erwartete Verhalten? In den folgenden empfohlenen Ressourcen finden Sie Leitfäden für verschiedene Probleme mit Richtlinien:</span><span class="sxs-lookup"><span data-stu-id="70499-103">Azure Information Protection: Policies not behaving as expected, see the following for recommended guidelines for various policy issues:</span></span>

1. <span data-ttu-id="70499-104">Wenn Probleme mit visuellen Markierungen auftreten, lesen Sie [Wann visuelle Markierungen angewendet werden](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span><span class="sxs-lookup"><span data-stu-id="70499-104">If you are having issues with visual markings, please review [When visual markings are applied](https://docs.microsoft.com/azure/information-protection/configure-policy-markings#when-visual-markings-are-applied).</span></span>
2. <span data-ttu-id="70499-105">Wenn Sie Probleme mit der automatischen Bezeichnung haben, lesen Sie [Konfigurieren von Bedingungen für die automatische und empfohlene Klassifizierung für Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) und [Wonach die Typen von vertraulichen Informationen suchen](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span><span class="sxs-lookup"><span data-stu-id="70499-105">If you are having issues with automatic labeling, please review [How to configure conditions for automatic and recommended classification for Azure Information Protection](https://docs.microsoft.com/azure/information-protection/configure-policy-classification) and [What the sensitive information types look for](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions).</span></span>
3. <span data-ttu-id="70499-106">Wenn es Probleme mit dem nativen/Datei-Schutz gibt, lesen Sie [Datei-API-Konfiguration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span><span class="sxs-lookup"><span data-stu-id="70499-106">If you are having issues with Native/Pfile protection, please review [File API configuration](https://docs.microsoft.com/azure/information-protection/develop/file-api-configuration).</span></span>
4. <span data-ttu-id="70499-107">Überprüfen Sie, ob Sie nicht ordnungsgemäß konfigurierte, bereichsbezogene Richtlinien verwenden: [Konfigurieren der Azure Information Protection-Richtlinie für bestimmte Benutzer mithilfe von bereichsbezogenen Richtlinien](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span><span class="sxs-lookup"><span data-stu-id="70499-107">Check if you are using scoped policies that aren't configured properly: [How to configure the Azure Information Protection policy for specific users by using scoped policies](https://docs.microsoft.com/azure/information-protection/configure-policy-scope).</span></span>
5. <span data-ttu-id="70499-108">Wenn die automatische Bezeichnung beim Anfügen eines mit einer Bezeichnung versehenen Dokuments in Outlook nicht funktioniert, überprüfen Sie, ob DRMEncryptProperty nicht etwa wie hier beschrieben definiert ist: [IRM-Registrierungseinstellungen für Sicherheit](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span><span class="sxs-lookup"><span data-stu-id="70499-108">If automatic labeling isn't working for Outlook when attaching a labeled document, verify that DRMEncryptProperty isn't defined as described here: [IRM registry settings for security](https://docs.microsoft.com/deployoffice/security/protect-sensitive-messages-and-documents-by-using-irm-in-office#office-2016-irm-registry-key-options).</span></span>

<span data-ttu-id="70499-109">Wenn weiterhin Probleme auftreten, rufen Sie Azure Information Protection-Clientprotokolle ab, und fügen Sie die exportierten Protokolle an dieses Ticket an.</span><span class="sxs-lookup"><span data-stu-id="70499-109">If you still are experiencing issues, please collect Azure Information Protection client logs and attach the exported logs to this ticket.</span></span>

1. <span data-ttu-id="70499-110">Öffnen Sie ein Office-Dokument oder erstellen Sie eine neue E-Mail in Outlook.</span><span class="sxs-lookup"><span data-stu-id="70499-110">Open an Office document or create a new email in Outlook.</span></span>
2. <span data-ttu-id="70499-111">Klicken Sie auf **Schutz/Vertraulichkeit** > **Hilfe und Feedback**.</span><span class="sxs-lookup"><span data-stu-id="70499-111">Click **Protect/Sensitivity** > **Help and feedback**.</span></span>
3. <span data-ttu-id="70499-112">Klicken Sie auf **Protokolle exportieren**.</span><span class="sxs-lookup"><span data-stu-id="70499-112">Click **Export Logs**.</span></span>
4. <span data-ttu-id="70499-113">Speichern Sie die Protokolle an einem beliebigen Ort, und fügen Sie sie an diese Serviceanfrage an.</span><span class="sxs-lookup"><span data-stu-id="70499-113">Save the logs to your choice of location, and attach them to this service request.</span></span>

<span data-ttu-id="70499-114">Zusätzliche Ressourcen:</span><span class="sxs-lookup"><span data-stu-id="70499-114">Additional resources:</span></span>

- [<span data-ttu-id="70499-115">Konfigurieren einer Bezeichnung für visuelle Markierungen für Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="70499-115">How to configure a label for visual markings for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-markings)
- [<span data-ttu-id="70499-116">Nachschlagen in der Azure Information Protection-Dokumentation</span><span class="sxs-lookup"><span data-stu-id="70499-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="70499-117">Verwenden von Vertraulichkeitsbezeichnungen in Microsoft 365-Apps</span><span class="sxs-lookup"><span data-stu-id="70499-117">Use sensitivity labels in Microsoft 365 apps</span></span>](https://docs.microsoft.com/microsoft-365/compliance/sensitivity-labels-office-apps)

