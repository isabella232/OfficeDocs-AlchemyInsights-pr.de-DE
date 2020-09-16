---
title: Datei schreibgeschützt geöffnet
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 2fdb4f048c2bee022a49c2cca2ce9770f42a87a2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745581"
---
# <a name="file-open-read-only"></a><span data-ttu-id="fa2fa-102">Datei schreibgeschützt geöffnet</span><span class="sxs-lookup"><span data-stu-id="fa2fa-102">File open read-only</span></span>

<span data-ttu-id="fa2fa-103">Sie können feststellen, dass beim Öffnen von Dateien schreibgeschützt geöffnet werden.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="fa2fa-104">In einigen Fällen ist dies für zusätzliche Sicherheit, beispielsweise beim Öffnen von Dateien aus dem Internet und anderen Zeiten, kann dies auf eine Einstellung zurückzuführen sein, die geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="fa2fa-105">Im folgenden finden Sie einige Szenarien, in denen eine Datei schreibgeschützt geöffnet wird, und einige Schritte, die Sie ausführen können, um dies zu ändern.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="fa2fa-106">**Mein Antivirus veranlasst das Öffnen eines schreibgeschützten**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="fa2fa-107">Einige Antiviren-Programme schützen Sie möglicherweise vor potenziell unsicheren Dateien, indem Sie sie schreibgeschützt öffnen.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="fa2fa-108">Sie müssen sich möglicherweise mit Ihrem Antivirus-Anbieter erkundigen, um zu erfahren, wie Sie diese Einstellungen anpassen.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="fa2fa-109">BitDefender enthält beispielsweise Inhalte zum Hinzufügen von Anwendungs Ausschlüssen hier: [Hinzufügen von Anwendungs-oder Prozess Ausschlüssen in BitDefender Control Center](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="fa2fa-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="fa2fa-110">**Sind die Dateieigenschaften auf schreibgeschützt festgelegt?**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="fa2fa-111">Sie können die Dateieigenschaften überprüfen, indem Sie mit der rechten Maustaste auf die Datei klicken und Eigenschaften auswählen.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="fa2fa-112">Wenn das schreibgeschützte Attribut aktiviert ist, können Sie es deaktivieren und auf OK klicken.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="fa2fa-113">**Der Inhalt befindet sich in der geschützten Ansicht.**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="fa2fa-114">Dateien aus dem Internet und aus anderen potenziell unsicheren Speicherorten können Viren, Würmer oder andere Arten von Schadsoftware enthalten, die Ihren Computer schädigen können.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="fa2fa-115">Dies ist auch häufig der Fall bei e-Mail-Anlagen oder Dateien, die Sie heruntergeladen haben.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="fa2fa-116">Zur Unterstützung des Schutzes Ihres Computers werden Dateien aus diesen potenziell unsicheren Speicherorten in der geschützten Ansicht geöffnet.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="fa2fa-117">Mithilfe der geschützten Ansicht können Sie eine Datei lesen und deren Inhalt anzeigen, während Sie die Risiken verringern.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="fa2fa-118">Weitere Informationen zur geschützten Ansicht und zum Ändern der Einstellungen finden Sie in diesem Artikel: [Was ist die geschützte Ansicht?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="fa2fa-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="fa2fa-119">**Ist OneDrive voll?**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="fa2fa-120">Wenn die Datei auf OneDrive gespeichert ist und Ihr OneDrive-Speicherplatz voll ist, können Sie das Dokument erst speichern, wenn Sie sich unter Ihrem zugewiesenen Speicherplatz befinden.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="fa2fa-121">Sie können Ihren freien Speicherplatz auf OneDrive überprüfen, indem Sie im Infocenter auf das OneDrive-Symbol klicken und Speicher verwalten auswählen, oder Sie können zu [https://onedrive.live.com](https://onedrive.live.com) , anmelden und die Menge des verwendeten Speicherplatzes in der linken oberen Ecke des Bildschirms wechseln.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="fa2fa-122">**Ist Office aktiviert?**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="fa2fa-123">Wenn Office nicht aktiviert ist oder Ihr Abonnement abgelaufen ist, können Sie den schreibgeschützten Modus für eingeschränkte Funktionen haben.</span><span class="sxs-lookup"><span data-stu-id="fa2fa-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="fa2fa-124">Informationen zum Aktivieren von Office finden Sie unter: nicht [lizenziertes Produkt und Aktivierungsfehler in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="fa2fa-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="fa2fa-125">**Wenn alles andere fehlschlägt...**</span><span class="sxs-lookup"><span data-stu-id="fa2fa-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="fa2fa-126">Versuchen Sie, den Computer neu zu starten</span><span class="sxs-lookup"><span data-stu-id="fa2fa-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="fa2fa-127">Installieren von Office-Updates</span><span class="sxs-lookup"><span data-stu-id="fa2fa-127">Install Office updates</span></span>
    
- <span data-ttu-id="fa2fa-128">Durchführen einer Online Reparatur von Office</span><span class="sxs-lookup"><span data-stu-id="fa2fa-128">Perform an Online repair of Office</span></span>
    

