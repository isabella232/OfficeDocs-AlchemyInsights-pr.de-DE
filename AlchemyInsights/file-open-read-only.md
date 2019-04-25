---
title: Schreibgeschütztes Datei öffnen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 4/26/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.openlocfilehash: 2b7f27e38412fc2a1dea46027e926c660231ed8b
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32401358"
---
# <a name="file-open-read-only"></a><span data-ttu-id="9847c-102">Schreibgeschütztes Datei öffnen</span><span class="sxs-lookup"><span data-stu-id="9847c-102">File open read-only</span></span>

<span data-ttu-id="9847c-103">Wenn Sie Dateien öffnen, werden Sie möglicherweise als schreibgeschützt geöffnet.</span><span class="sxs-lookup"><span data-stu-id="9847c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="9847c-104">In einigen Fällen gilt dies für zusätzliche Sicherheit, beispielsweise beim Öffnen von Dateien aus dem Internet und anderen Zeiten, kann dies auf eine Einstellung zurückzuführen sein, die geändert werden kann.</span><span class="sxs-lookup"><span data-stu-id="9847c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="9847c-105">Hier sind einige Szenarios, in denen eine Datei schreibgeschützt geöffnet wird, und einige Schritte, die Sie ausführen können, um dies zu ändern.</span><span class="sxs-lookup"><span data-stu-id="9847c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="9847c-106">**Mein Antivirus bewirkt, dass Sie schreibgeschützt öffnen**</span><span class="sxs-lookup"><span data-stu-id="9847c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="9847c-107">Einige Antivirenprogramme schützen Sie möglicherweise vor potenziell unsicheren Dateien, indem Sie diese schreibgeschützt öffnen.</span><span class="sxs-lookup"><span data-stu-id="9847c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="9847c-108">Möglicherweise müssen Sie sich beim Antivirus-Anbieter erkundigen, wie Sie diese Einstellungen anpassen.</span><span class="sxs-lookup"><span data-stu-id="9847c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="9847c-109">BitDefender hat beispielsweise Inhalte zum Hinzufügen von Anwendungs Ausschlüssen hier: [Hinzufügen von Anwendungs-oder Prozess Ausschlüssen in BitDefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span><span class="sxs-lookup"><span data-stu-id="9847c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://www.bitdefender.com/support/how-to-add-application-or-process-exclusions-in-bitdefender-control-center-1119.mdl).</span></span>
  
 <span data-ttu-id="9847c-110">**Sind die Dateieigenschaften auf schreibgeschützt festgelegt?**</span><span class="sxs-lookup"><span data-stu-id="9847c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="9847c-111">Sie können die Dateieigenschaften überprüfen, indem Sie mit der rechten Maustaste auf die Datei klicken und Eigenschaften auswählen.</span><span class="sxs-lookup"><span data-stu-id="9847c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="9847c-112">Wenn das Read-only-Attribut aktiviert ist, können Sie es deaktivieren und auf OK klicken.</span><span class="sxs-lookup"><span data-stu-id="9847c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="9847c-113">**Der Inhalt befindet sich in der geschützten Ansicht**</span><span class="sxs-lookup"><span data-stu-id="9847c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="9847c-114">Dateien aus dem Internet und aus anderen potenziell unsicheren Speicherorten können Viren, Würmer oder andere Arten von Schadsoftware enthalten, die Ihren Computer schädigen können.</span><span class="sxs-lookup"><span data-stu-id="9847c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="9847c-115">Dies gilt häufig auch für e-Mail-Anhänge oder Dateien, die Sie heruntergeladen haben.</span><span class="sxs-lookup"><span data-stu-id="9847c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="9847c-116">Um Ihren Computer zu schützen, werden Dateien aus diesen potenziell unsicheren Speicherorten in der geschützten Ansicht geöffnet.</span><span class="sxs-lookup"><span data-stu-id="9847c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="9847c-117">Mithilfe der geschützten Ansicht können Sie eine Datei lesen und deren Inhalt anzeigen, während Sie die Risiken reduzieren.</span><span class="sxs-lookup"><span data-stu-id="9847c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="9847c-118">Weitere Informationen zur geschützten Ansicht und zum Ändern der Einstellungen finden Sie in diesem Artikel: [Was ist geschützte Ansicht?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="9847c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="9847c-119">**Ist OneDrive voll?**</span><span class="sxs-lookup"><span data-stu-id="9847c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="9847c-120">Wenn die Datei in OneDrive gespeichert ist und Ihr OneDrive-Speicherplatz voll ist, können Sie das Dokument erst speichern, wenn Sie den zugewiesenen Speicherplatz belegt haben.</span><span class="sxs-lookup"><span data-stu-id="9847c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="9847c-121">Sie können Ihren freien Speicherplatz auf OneDrive überprüfen, indem Sie auf das OneDrive-Symbol im Notification Center klicken und die Option Speicher verwalten [http://onedrive.live.com](http://onedrive.live.com)auswählen, oder Sie wechseln zu, melden Sie sich an, und notieren Sie sich die Menge des verwendeten Speicherplatzes in der unteren linken Ecke des Bildschirms.</span><span class="sxs-lookup"><span data-stu-id="9847c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [http://onedrive.live.com](http://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="9847c-122">**Ist Office aktiviert?**</span><span class="sxs-lookup"><span data-stu-id="9847c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="9847c-123">Wenn Office nicht aktiviert ist oder Ihr Abonnement abgelaufen ist, können Sie den schreibgeschützten Modus "reduzierte Funktionalität" nutzen.</span><span class="sxs-lookup"><span data-stu-id="9847c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="9847c-124">Informationen zum Aktivieren von Office finden Sie unter: nicht [lizenzierte Produkte und Aktivierungsfehler in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="9847c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="9847c-125">**Wenn alle anderen Fehler auftreten...**</span><span class="sxs-lookup"><span data-stu-id="9847c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="9847c-126">Neustarten des Computers</span><span class="sxs-lookup"><span data-stu-id="9847c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="9847c-127">Installieren von Office-Updates</span><span class="sxs-lookup"><span data-stu-id="9847c-127">Install Office updates</span></span>
    
- <span data-ttu-id="9847c-128">Durchführen einer Online Reparatur von Office</span><span class="sxs-lookup"><span data-stu-id="9847c-128">Perform an Online repair of Office</span></span>
    

