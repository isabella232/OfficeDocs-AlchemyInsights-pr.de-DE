---
title: Problem beim Öffnen oder Herunterladen von Dateien in Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695648"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a><span data-ttu-id="636d2-102">Problem beim Öffnen oder Herunterladen von Dateien in Yammer</span><span class="sxs-lookup"><span data-stu-id="636d2-102">Issue opening or downloading files in Yammer</span></span>

<span data-ttu-id="636d2-103">Das klassische Yammer unterstützt mehrere Optionen für das Hochladen von Dateien in Nachrichten und Gruppen.</span><span class="sxs-lookup"><span data-stu-id="636d2-103">Classic Yammer supports multiple option for file uploads to messages and groups.</span></span> <span data-ttu-id="636d2-104">Je nach Netzwerkkonfiguration sind Dateien standardmäßig in SharePoint gespeichert.</span><span class="sxs-lookup"><span data-stu-id="636d2-104">Depending on network configuration, files default to storage in SharePoint.</span></span>

<span data-ttu-id="636d2-105">Die Dateiauswahl im neuen Yammer unterstützt noch nicht alle Optionen, die im klassischen Yammer zur Verfügung stehen.</span><span class="sxs-lookup"><span data-stu-id="636d2-105">The file picker in new Yammer does not yet support all the options available in classic Yammer.</span></span> <span data-ttu-id="636d2-106">Ein zukünftiges Update wird weitere Features hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="636d2-106">A future update will add additional features.</span></span> <span data-ttu-id="636d2-107">Weitere Informationen hierzu finden Sie unter [Anfügen einer Datei oder eines Bilds an einen Beitrag in einer Yammer-Unterhaltung](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span><span class="sxs-lookup"><span data-stu-id="636d2-107">For more info, see [Attach a file or image to a Yammer conversation post](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8).</span></span>

<span data-ttu-id="636d2-108">**Datei kann nicht geöffnet oder heruntergeladen werden**</span><span class="sxs-lookup"><span data-stu-id="636d2-108">**Unable to open or download a file**</span></span>  

<span data-ttu-id="636d2-109">Eine Datei kann in Yammer hochgeladen werden, aber zusätzlich auf eine Datei in SharePoint Online verlinkt sein.</span><span class="sxs-lookup"><span data-stu-id="636d2-109">A file might upload to Yammer but also be linking to a file in SharePoint Online.</span></span> <span data-ttu-id="636d2-110">Zur Problembehandlung müssen Sie zuerst den Speicherort der Datei ermitteln.</span><span class="sxs-lookup"><span data-stu-id="636d2-110">To troubleshoot, first you must determine the location of the file.</span></span> <span data-ttu-id="636d2-111">Wenn die Datei in Yammer hochgeladen wurde, weist sie eine \*.yammer.com-URL auf.</span><span class="sxs-lookup"><span data-stu-id="636d2-111">If the file has been uploaded to Yammer, it will have a \*.yammer.com URL.</span></span> <span data-ttu-id="636d2-112">Stellen Sie sicher, dass erforderliche URLs und IP-Adressen nicht blockiert werden.</span><span class="sxs-lookup"><span data-stu-id="636d2-112">Ensure that required URLs and IP addresses are unblocked.</span></span> <span data-ttu-id="636d2-113">Weitere Informationen hierzu finden Sie im Blogbeitrag [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span><span class="sxs-lookup"><span data-stu-id="636d2-113">For more info, see the blog post [Using hard coded IP addresses for Yammer is not recommended](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592).</span></span>

<span data-ttu-id="636d2-114">Überprüfen Sie, ob ein Benutzer, der auch ein globaler Administrator ist, die Datei herunterladen kann.</span><span class="sxs-lookup"><span data-stu-id="636d2-114">Check whether a user who is also a global admin can download the file.</span></span> <span data-ttu-id="636d2-115">Ist die Datei privat, müssen Sie möglicherweise den Modus für private Inhalte verwenden.</span><span class="sxs-lookup"><span data-stu-id="636d2-115">If the file is private, you might have to use Private Content Mode.</span></span> <span data-ttu-id="636d2-116">Weitere Informationen finden Sie unter [Überwachen privater Inhalte in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span><span class="sxs-lookup"><span data-stu-id="636d2-116">For more info, see then [Monitor private content in Yammer](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content).</span></span>  

<span data-ttu-id="636d2-117">**Gäste und Dateien auf Yammer-Netzwerkebene in SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="636d2-117">**Yammer network-level guests and files in SharePoint Online**</span></span>  

<span data-ttu-id="636d2-118">[Gäste auf Yammer-Netzwerkebene](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) verwenden kein Azure AD B2B und sind für den Yammer-Dienst interne Benutzer, daher können Sie auf in SharePoint gespeicherte Yammer-Dateien nicht zugreifen.</span><span class="sxs-lookup"><span data-stu-id="636d2-118">[Network-level guests in Yammer](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) do not use Azure AD B2B and are internal to the Yammer service, so they can't access Yammer files stored in SharePoint.</span></span> <span data-ttu-id="636d2-119">Erstellen Sie einen externen AAD-B2B-Benutzer, der unter Verwendung dieser Identität auf Dokumentbibliotheken in SharePoint Online zugreifen kann.</span><span class="sxs-lookup"><span data-stu-id="636d2-119">Create an external AAD B2B user who can access document libraries in SharePoint Online by using that identity.</span></span> <span data-ttu-id="636d2-120">Informationen zur künftigen Azure AD B2B-Gastunterstützung in Yammer finden Sie unter [Business-to-Business (B2B) – Gast Support in Yammer, Vorschau – Kundenbedingungen und häufig gestellte Fragen (FAQ)](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span><span class="sxs-lookup"><span data-stu-id="636d2-120">For information about future Azure AD B2B guest support in Yammer, see [Business-to-business (B2B) Guest support in Yammer Preview - Customer Terms and FAQ](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer).</span></span>