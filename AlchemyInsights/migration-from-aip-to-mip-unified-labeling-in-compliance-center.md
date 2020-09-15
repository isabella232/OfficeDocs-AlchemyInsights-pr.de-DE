---
title: Migration von AIP zu MIP/einheitlichen Bezeichnungen im Compliance Center
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674325"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a><span data-ttu-id="a2f86-102">Migration von AIP zu MIP/einheitlichen Bezeichnungen im Compliance Center</span><span class="sxs-lookup"><span data-stu-id="a2f86-102">Migration from AIP to MIP/Unified Labeling in the Compliance Center</span></span>

<span data-ttu-id="a2f86-103">Um von AIP-Bezeichnungen zu einheitlichen Bezeichnungen im Security & Compliance Center zu migrieren, gehen Sie folgendermaßen vor:</span><span class="sxs-lookup"><span data-stu-id="a2f86-103">To migrate from AIP labels to Unified Labeling in the Security and Compliance center, do the following:</span></span>

<span data-ttu-id="a2f86-104">**Aktivieren Sie den Schutz über das Azure-Portal**</span><span class="sxs-lookup"><span data-stu-id="a2f86-104">**Activate protection from the Azure portal**</span></span>

1. <span data-ttu-id="a2f86-105">Wenn Sie dies noch nicht getan haben, öffnen Sie ein neues Browserfenster, und [melden Sie sich beim Azure-Portal an](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span><span class="sxs-lookup"><span data-stu-id="a2f86-105">If you haven't already done so, open a new browser window and [sign in to the Azure portal](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal).</span></span> <span data-ttu-id="a2f86-106">Navigieren Sie zum Blatt **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="a2f86-106">Navigate to the **Azure Information Protection** blade.</span></span> <span data-ttu-id="a2f86-107">Klicken Sie z. B. im Hubmenü auf **Alle Dienste**, und beginnen Sie mit der Eingabe von **Informationen** im Feld "Filter".</span><span class="sxs-lookup"><span data-stu-id="a2f86-107">For example, on the hub menu, click **All services** and start typing **Information** in the Filter box.</span></span> <span data-ttu-id="a2f86-108">Wählen Sie **Azure Information Protection** aus.</span><span class="sxs-lookup"><span data-stu-id="a2f86-108">Select **Azure Information Protection**.</span></span> <span data-ttu-id="a2f86-109">Wenn Sie bisher noch nicht auf das Blatt "Azure Information Protection" zugegriffen haben, lesen Sie die einmaligen [zusätzlichen Schritte](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time), um dieses Blatt zum Portal hinzuzufügen.</span><span class="sxs-lookup"><span data-stu-id="a2f86-109">If you haven't accessed the Azure Information Protection blade before, see the one-time [additional steps](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) to add this blade to the portal.</span></span> <span data-ttu-id="a2f86-110">Um das Blatt "Azure Information Protection" zu öffnen, müssen Sie über einen [Azure Information Protection Premium-Plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) oder einen Office 365-Plan verfügen, der die Rechteverwaltung umfasst.</span><span class="sxs-lookup"><span data-stu-id="a2f86-110">To open the Azure Information Protection blade, you must have either an [Azure Information Protection Premium plan](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) or an Office 365 plan that includes Rights Management.</span></span> <span data-ttu-id="a2f86-111">Wenn Sie über eines dieser Abonnements verfügen, aber eine Nachricht erhalten, dass kein gültiges Abonnement gefunden wird, [wenden Sie sich an den Microsoft-Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support), oder verwenden Sie unsere Standardsupportkanäle.</span><span class="sxs-lookup"><span data-stu-id="a2f86-111">If you have one of these subscriptions but see a message that a valid subscription cannot be found, [contact Microsoft Support](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) or use your standard support channels.</span></span>

2. <span data-ttu-id="a2f86-112">Suchen Sie die Menüoptionen **Verwalten**, und wählen Sie **Schutzaktivierung** aus.</span><span class="sxs-lookup"><span data-stu-id="a2f86-112">Locate the **Manage** menu options, and select **Protection activation**.</span></span> <span data-ttu-id="a2f86-113">Klicken Sie auf **Aktivieren**, und bestätigen Sie dann Ihre Aktion.</span><span class="sxs-lookup"><span data-stu-id="a2f86-113">Click **Activate**, and then confirm your action.</span></span> <span data-ttu-id="a2f86-114">Nach Abschluss der Aktivierung wird auf der Informationsleiste **Aktivierung erfolgreich abgeschlossen** angezeigt.</span><span class="sxs-lookup"><span data-stu-id="a2f86-114">When activation is complete, the information bar displays **Activation finished successfully**.</span></span>

<span data-ttu-id="a2f86-115">**Migrieren von Azure Information Protection-Bezeichnungen zum Office 365 Security & Compliance Center**</span><span class="sxs-lookup"><span data-stu-id="a2f86-115">**Migrate Azure Information Protection labels to Office 365 Security & Compliance Center**</span></span>

1. <span data-ttu-id="a2f86-116">Stellen Sie sicher, dass Sie als Benutzer mit globalen Administratorberechtigungen angemeldet sind.</span><span class="sxs-lookup"><span data-stu-id="a2f86-116">Make sure you are logged in as a user with Global Administrator permission.</span></span>

2. <span data-ttu-id="a2f86-117">Navigieren Sie zum Blatt **Azure Information Protection**.</span><span class="sxs-lookup"><span data-stu-id="a2f86-117">Navigate to the **Azure Information Protection** blade.</span></span>

3. <span data-ttu-id="a2f86-118">Wählen Sie aus der Menüoption **Verwalten** die Option **Einheitliche Bezeichnungen** aus.</span><span class="sxs-lookup"><span data-stu-id="a2f86-118">From the **Manage** menu option, select **Unified labeling**.</span></span>

4. <span data-ttu-id="a2f86-119">Klicken Sie auf dem Blatt **Azure Information Protection – Einheitliche Bezeichnungen** auf **Aktivieren**, und folgen Sie den Onlineanweisungen.</span><span class="sxs-lookup"><span data-stu-id="a2f86-119">On the **Azure Information Protection - Unified labeling** blade, click **Activate** and follow the online instructions.</span></span>

<span data-ttu-id="a2f86-120">**Hinweis**: Vergewissern Sie sich, dass Sie über die entsprechenden Berechtigungen verfügen, bevor Sie die Security & Compliance Center-Migration aktivieren.</span><span class="sxs-lookup"><span data-stu-id="a2f86-120">**Note**: Verify that you have the appropriate permissions before activating the Security & Compliance Center Migration.</span></span> <span data-ttu-id="a2f86-121">Weitere Informationen finden Sie in diesen Artikeln:</span><span class="sxs-lookup"><span data-stu-id="a2f86-121">See these articles for more info:</span></span>

1. [<span data-ttu-id="a2f86-122">Benötigt man globale Administratorrechte, um Azure Information Protection zu konfigurieren, oder kann ich das an andere Administratoren delegieren?</span><span class="sxs-lookup"><span data-stu-id="a2f86-122">Do you need to be a global admin to configure Azure Information Protection, or can I delegate to other administrators?</span></span>](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [<span data-ttu-id="a2f86-123">Wichtige Informationen über administrative Rollen nach der Migration zum Security & Compliance Center</span><span class="sxs-lookup"><span data-stu-id="a2f86-123">Important information about administrative roles after migrating to Security & Compliance Center.</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

<span data-ttu-id="a2f86-124">Weitere Informationen über die Migration von AIP zu einheitlichen Bezeichnungen zum Security & Compliance Center finden Sie unter [Migrieren von Bezeichnungen](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span><span class="sxs-lookup"><span data-stu-id="a2f86-124">For more information on the AIP to Unified Labeling migration to Security and Compliance Center, see [Migrate labels](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).</span></span>
