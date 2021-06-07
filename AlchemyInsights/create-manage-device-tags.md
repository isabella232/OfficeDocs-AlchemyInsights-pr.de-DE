---
title: Erstellen und Verwalten von Gerätekategorien oder -gruppen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721698"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="ff12d-102">Erstellen und Verwalten von Gerätekategorien oder -gruppen</span><span class="sxs-lookup"><span data-stu-id="ff12d-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="ff12d-103">Fügen Sie Kategorien auf Geräten hinzu, um eine logische Gruppenzugehörigkeit zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="ff12d-104">Gerätekategorien unterstützen die ordnungsgemäße Zuordnung des Netzwerks, sodass Sie verschiedene Kategorien anfügen können, um den Kontext zu erfassen und die dynamische Listenerstellung als Teil eines Vorfalls zu ermöglichen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="ff12d-105">Kategorien können als Filter in der Listenansicht für Geräte oder zum Gruppieren von Geräten verwendet werden.</span><span class="sxs-lookup"><span data-stu-id="ff12d-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="ff12d-106">Weitere Informationen zum Gruppieren von Geräten finden Sie unter [Erstellen und Verwalten von Gerätekategorien](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="ff12d-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="ff12d-107">Sie können Kategorien auf Geräten hinzufügen, indem Sie:</span><span class="sxs-lookup"><span data-stu-id="ff12d-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="ff12d-108">Das Portal verwenden</span><span class="sxs-lookup"><span data-stu-id="ff12d-108">Using the portal</span></span>

- <span data-ttu-id="ff12d-109">Einen Registrierungsschlüsselwert festlegen</span><span class="sxs-lookup"><span data-stu-id="ff12d-109">Setting a registry key value</span></span>
 
<span data-ttu-id="ff12d-110">**Hinweis:** Zwischen dem Zeitpunkt, zu dem eine Kategorie zu einem Gerät hinzugefügt wird und wann sie in der Geräteliste und auf der Geräteseite verfügbar ist, kann es zu Wartezeiten kommen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="ff12d-111">Informationen zum Hinzufügen von Gerätekategorien mithilfe der API finden Sie unter [Hinzufügen oder Entfernen von Gerätekategorien-API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span><span class="sxs-lookup"><span data-stu-id="ff12d-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="ff12d-112">Hinzufügen und Verwalten von Gerätekategorien über das Portal</span><span class="sxs-lookup"><span data-stu-id="ff12d-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="ff12d-113">Wählen Sie das Gerät aus, auf dem Sie Kategorien verwalten möchten.</span><span class="sxs-lookup"><span data-stu-id="ff12d-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="ff12d-114">Sie können ein Gerät aus einer der folgenden Ansichten auswählen oder danach suchen:</span><span class="sxs-lookup"><span data-stu-id="ff12d-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="ff12d-115">**Dashboard für Sicherheitsvorgänge** Wählen Sie den Gerätenamen im Abschnitt "Top-Geräte mit aktiven Benachrichtigungen" aus.</span><span class="sxs-lookup"><span data-stu-id="ff12d-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="ff12d-116">**Benachrichtigungswarteschlange** – Wählen Sie den Gerätenamen neben dem Gerätesymbol aus der Benachrichtigungswarteschlange aus.</span><span class="sxs-lookup"><span data-stu-id="ff12d-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="ff12d-117">**Geräteliste** – Wählen Sie den Gerätenamen aus der Geräteliste aus.</span><span class="sxs-lookup"><span data-stu-id="ff12d-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="ff12d-118">**Suchfeld** – Wählen Sie im Dropdownmenü "Gerät" aus und geben Sie den Gerätenamen ein.</span><span class="sxs-lookup"><span data-stu-id="ff12d-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="ff12d-119">Sie können die Benachrichtigungsseite auch über die Datei- und IP-Ansichten öffnen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="ff12d-120">Wählen Sie **Kategorien verwalten** aus der Zeile "Antwortaktionen" aus.</span><span class="sxs-lookup"><span data-stu-id="ff12d-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="ff12d-121">Geben Sie Text ein, um Kategorien zu suchen oder zu erstellen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-121">Type to find or create tags.</span></span>

<span data-ttu-id="ff12d-122">Kategorien werden der Geräteansicht hinzugefügt und in der Listenansicht für Geräte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="ff12d-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="ff12d-123">Anschließend können Sie mithilfe des Kategorienfilters die relevante Geräteliste anzeigen.</span><span class="sxs-lookup"><span data-stu-id="ff12d-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="ff12d-124">Weitere Informationen finden Sie unter [Erstellen und Verwalten von Gerätekategorien](/microsoft-365/security/defender-endpoint/machine-tags).</span><span class="sxs-lookup"><span data-stu-id="ff12d-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>