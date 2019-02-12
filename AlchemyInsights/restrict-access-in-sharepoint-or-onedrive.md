---
title: Einschränken des Zugriffs auf SharePoint- und OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e0fbec6eb269a173664e2b9a1efe6eefb527b96f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 02/12/2019
ms.locfileid: "29905147"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="92bac-102">Einschränken des Zugriffs auf SharePoint- und OneDrive</span><span class="sxs-lookup"><span data-stu-id="92bac-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="92bac-p101">In SharePoint und OneDrive schränken Sie den Zugriff auf Elemente wie Dateien, Ordner und Listen durch Gewähren von Zugriff nur für Gruppen oder Einzelpersonen, die Sie Zugriff gewähren möchten. Standardmäßig werden Berechtigungen in SharePoint höhere oben in der Hierarchie geerbt. Also: eine Datei erbt die Berechtigungen aus dem Ordner, der die Berechtigungen aus der Bibliothek erbt, die ihre Berechtigungen von der Website erbt.</span><span class="sxs-lookup"><span data-stu-id="92bac-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="92bac-p102">Sie können auf einer höheren Ebene freigeben (wie durch die gemeinsame Nutzung einer gesamten Website), und klicken Sie dann Vererbung unterbrechen, wenn Sie nicht alle Elemente auf der Website freigeben möchten. Jedoch empfohlen nicht, da es ermöglicht die Verwaltung von den Berechtigungen komplexere und verwirrend in der Zukunft. Nachfolgend finden Sie stattdessen möglich:</span><span class="sxs-lookup"><span data-stu-id="92bac-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="92bac-109">Wenn Sie beispielsweise die Inhalte eines Ordners mit Ausnahme einer Datei in diesem Ordner freigeben möchten, verschieben Sie diese Datei an einen neuen Speicherort an, der nicht freigegeben ist.</span><span class="sxs-lookup"><span data-stu-id="92bac-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="92bac-110">Wenn Sie zwei Unterordner in einem Ordner haben, und Sie einen Unterordner für die Gruppen A und B freigeben und nur eine Gruppenzugriff auf den zweiten Unterordner zulassen, Freigeben des übergeordneten Ordners für Gruppe A und Gruppe B in der ersten Unterordner hinzufügen möchten.</span><span class="sxs-lookup"><span data-stu-id="92bac-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="92bac-111">Beenden der Freigabe einer Datei oder eines Ordners</span><span class="sxs-lookup"><span data-stu-id="92bac-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

