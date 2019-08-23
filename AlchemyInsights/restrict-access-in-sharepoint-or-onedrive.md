---
title: Einschränken des Zugriffs in SharePoint oder OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551450"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d9d23-102">Einschränken des Zugriffs in SharePoint oder OneDrive</span><span class="sxs-lookup"><span data-stu-id="d9d23-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d9d23-103">In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen ein, indem Sie nur Gruppen oder Personen Zugriff gewähren, auf die Sie Zugriff haben möchten.</span><span class="sxs-lookup"><span data-stu-id="d9d23-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="d9d23-104">Standardmäßig werden Berechtigungen in SharePoint von oben in der Hierarchie vererbt.</span><span class="sxs-lookup"><span data-stu-id="d9d23-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="d9d23-105">Eine Datei erbt also Ihre Berechtigungen aus dem Ordner, der Ihre Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.</span><span class="sxs-lookup"><span data-stu-id="d9d23-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="d9d23-106">Sie können auf einer höheren Ebene freigeben (beispielsweisedurch Freigabe einer ganzen Website) und dann die Vererbung aufbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten.</span><span class="sxs-lookup"><span data-stu-id="d9d23-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="d9d23-107">Dies wird jedoch nicht empfohlen, da die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird.</span><span class="sxs-lookup"><span data-stu-id="d9d23-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="d9d23-108">Hier sehen Sie, was Sie stattdessen tun könnten:</span><span class="sxs-lookup"><span data-stu-id="d9d23-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="d9d23-109">Wenn Sie beispielsweise alle Inhalte eines Ordners mit Ausnahme einer einzigen Datei freigeben möchten, müssen Sie die Datei an einen neuen Speicherort versetzen, der nicht freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="d9d23-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="d9d23-110">Wenn Sie über zwei Unterordner in einem Ordner verfügen und einen Unterordner mit den Gruppen a und B freigeben und nur Gruppen Zugriff auf den zweiten Unterordner zulassen möchten, geben Sie den übergeordneten Ordner mit Gruppe a frei, und fügen Sie Gruppe b dem ersten Unterordner hinzu.</span><span class="sxs-lookup"><span data-stu-id="d9d23-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="d9d23-111">Beenden der Freigabe einer Datei oder eines Ordners</span><span class="sxs-lookup"><span data-stu-id="d9d23-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

