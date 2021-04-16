---
title: Schreibgeschütztes Öffnen von Dateien
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813183"
---
# <a name="file-open-read-only"></a><span data-ttu-id="be97d-102">Schreibgeschütztes Öffnen von Dateien</span><span class="sxs-lookup"><span data-stu-id="be97d-102">File open read-only</span></span>

<span data-ttu-id="be97d-103">Sie können feststellen, dass beim Öffnen von Dateien diese schreibgeschützt geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="be97d-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="be97d-104">In einigen Fällen ist dies für zusätzliche Sicherheit, z. B. beim Öffnen von Dateien aus dem Internet, und in anderen Fällen kann dies auf eine Einstellung, die geändert werden kann, liegen.</span><span class="sxs-lookup"><span data-stu-id="be97d-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="be97d-105">Hier sind einige Szenarien, in denen eine Datei schreibgeschützt geöffnet wird, und einige Schritte, die Sie ausführen können, um dies zu ändern.</span><span class="sxs-lookup"><span data-stu-id="be97d-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="be97d-106">**My antivirus is causing them to open read-only**</span><span class="sxs-lookup"><span data-stu-id="be97d-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="be97d-107">Einige Antivirenprogramme schützen Sie möglicherweise vor potenziell unsicheren Dateien, indem sie schreibgeschützt geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="be97d-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="be97d-108">Möglicherweise müssen Sie sich bei Ihrem Antivirenanbieter informieren, um zu erfahren, wie Sie diese Einstellungen anpassen.</span><span class="sxs-lookup"><span data-stu-id="be97d-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="be97d-109">BitDefender enthält beispielsweise Inhalte zum Hinzufügen von Anwendungsausschlüssen hier: Hinzufügen von Anwendungs- oder [Prozessausschlüssen in Bitdefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="be97d-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="be97d-110">**Sind die Dateieigenschaften auf schreibgeschützt festgelegt?**</span><span class="sxs-lookup"><span data-stu-id="be97d-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="be97d-111">Sie können die Dateieigenschaften überprüfen, indem Sie mit der rechten Maustaste auf die Datei klicken und Eigenschaften auswählen.</span><span class="sxs-lookup"><span data-stu-id="be97d-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="be97d-112">Wenn das Attribut Schreibgeschützt aktiviert ist, können Sie es deaktivieren und auf OK klicken.</span><span class="sxs-lookup"><span data-stu-id="be97d-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="be97d-113">**Der Inhalt befindet sich in der geschützten Ansicht**</span><span class="sxs-lookup"><span data-stu-id="be97d-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="be97d-114">Dateien aus dem Internet und von anderen potenziell unsicheren Speicherorten können Viren, Würmer oder andere Arten von Schadsoftware enthalten, die Ihren Computer schädigen können.</span><span class="sxs-lookup"><span data-stu-id="be97d-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="be97d-115">Dies ist auch häufig bei E-Mail-Anlagen oder Dateien der Fall, die Sie heruntergeladen haben.</span><span class="sxs-lookup"><span data-stu-id="be97d-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="be97d-116">Um Ihren Computer zu schützen, werden Dateien vor diesen potenziell unsicheren Speicherorten in der geschützten Ansicht geöffnet.</span><span class="sxs-lookup"><span data-stu-id="be97d-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="be97d-117">Mithilfe der geschützten Ansicht können Sie eine Datei lesen und deren Inhalt anzeigen und gleichzeitig die Risiken verringern.</span><span class="sxs-lookup"><span data-stu-id="be97d-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="be97d-118">Weitere Informationen zur geschützten Ansicht und zum Ändern von Einstellungen finden Sie in diesem Artikel: [Was ist geschützte Ansicht?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="be97d-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="be97d-119">**Ist OneDrive voll?**</span><span class="sxs-lookup"><span data-stu-id="be97d-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="be97d-120">Wenn die Datei auf OneDrive gespeichert ist und Ihr #A0 voll ist, können Sie das Dokument erst speichern, wenn Sie sich unter Ihrem zugewiesenen Speicherplatz befinden.</span><span class="sxs-lookup"><span data-stu-id="be97d-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="be97d-121">Sie können Ihren freien Speicherplatz auf OneDrive überprüfen, indem Sie im Benachrichtigungscenter auf das #A0 klicken und Speicher verwalten auswählen, oder Sie können zu wechseln, sich anmelden und die Menge des verwendeten Speicherplatzes unten links auf dem Bildschirm [https://onedrive.live.com](https://onedrive.live.com) notieren.</span><span class="sxs-lookup"><span data-stu-id="be97d-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="be97d-122">**Ist Office aktiviert?**</span><span class="sxs-lookup"><span data-stu-id="be97d-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="be97d-123">Wenn Office nicht aktiviert ist oder Ihr Abonnement abgelaufen ist, können Sie sich im schreibgeschützten Modus mit eingeschränkter Funktionalität befinden.</span><span class="sxs-lookup"><span data-stu-id="be97d-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="be97d-124">Informationen zum Aktivieren von Office finden Sie unter: [Nicht lizenziertes Produkt und Aktivierungsfehler in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="be97d-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="be97d-125">**Wenn alle anderen Fehler nicht erfolgreich sind...**</span><span class="sxs-lookup"><span data-stu-id="be97d-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="be97d-126">Versuchen Sie, den Computer neu zu starten</span><span class="sxs-lookup"><span data-stu-id="be97d-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="be97d-127">Office-Updates installieren</span><span class="sxs-lookup"><span data-stu-id="be97d-127">Install Office updates</span></span>
    
- <span data-ttu-id="be97d-128">Durchführen einer Onlinereparatur von Office</span><span class="sxs-lookup"><span data-stu-id="be97d-128">Perform an Online repair of Office</span></span>
    

