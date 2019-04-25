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
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32383870"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="b6bad-102">Einschränken des Zugriffs in SharePoint oder OneDrive</span><span class="sxs-lookup"><span data-stu-id="b6bad-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="b6bad-103">In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen ein, indem Sie nur Gruppen oder Einzelpersonen Zugriff gewähren, auf die Sie zugreifen möchten.</span><span class="sxs-lookup"><span data-stu-id="b6bad-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="b6bad-104">Standardmäßig werden Berechtigungen in SharePoint von höher oben in der Hierarchie geerbt.</span><span class="sxs-lookup"><span data-stu-id="b6bad-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="b6bad-105">Eine Datei erbt daher ihre Berechtigungen vom Ordner, der Ihre Berechtigungen von der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.</span><span class="sxs-lookup"><span data-stu-id="b6bad-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="b6bad-106">Sie können auf einer höheren Ebene freigeben (beispielsweisedurch Freigeben einer gesamten Website) und dann die Vererbung unterbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten.</span><span class="sxs-lookup"><span data-stu-id="b6bad-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="b6bad-107">Dies wird jedoch nicht empfohlen, da dadurch die Verwaltung der Berechtigungen in Zukunft komplexer und verwirrender wird.</span><span class="sxs-lookup"><span data-stu-id="b6bad-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="b6bad-108">Stattdessen können Sie Folgendes tun:</span><span class="sxs-lookup"><span data-stu-id="b6bad-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="b6bad-109">Wenn Sie beispielsweise den gesamten Inhalt eines Ordners mit Ausnahme einer Datei freigeben möchten, verschieben Sie diese Datei an einen neuen Speicherort, der nicht freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="b6bad-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="b6bad-110">Wenn Sie zwei Unterordner in einem Ordner haben und einen Unterordner mit den Gruppen A und B freigeben möchten und nur den Gruppen Zugriff auf den zweiten Unterordner zulassen, teilen Sie den übergeordneten Ordner mit Gruppe A, und fügen Sie Gruppe B zum ersten Unterordner hinzu.</span><span class="sxs-lookup"><span data-stu-id="b6bad-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="b6bad-111">Beenden der Freigabe einer Datei oder eines Ordners</span><span class="sxs-lookup"><span data-stu-id="b6bad-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

