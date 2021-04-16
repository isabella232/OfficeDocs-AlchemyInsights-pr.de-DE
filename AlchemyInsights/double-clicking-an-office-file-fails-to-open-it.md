---
title: Doppelklicken auf eine Office-Datei kann nicht geöffnet werden
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2200002"
- "161"
ms.openlocfilehash: b9c563f7dd099bf3bad9018f69e2096816dd7290
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51814804"
---
# <a name="double-clicking-an-office-file-fails-to-open-it"></a><span data-ttu-id="7c636-102">Doppelklicken auf eine Office-Datei kann nicht geöffnet werden</span><span class="sxs-lookup"><span data-stu-id="7c636-102">Double-clicking an Office file fails to open it</span></span>

<span data-ttu-id="7c636-103">Nach dem Doppelklicken auf eine Office-Datei wird möglicherweise das Programm geöffnet, aber die Datei selbst wird nicht geöffnet.</span><span class="sxs-lookup"><span data-stu-id="7c636-103">After double-clicking an Office file, you may see the program open but the file itself doesn't open.</span></span> <span data-ttu-id="7c636-104">Oder Sie erhalten den Fehler: "Beim Senden des Befehls an das Programm ist ein Problem aufgetreten."</span><span class="sxs-lookup"><span data-stu-id="7c636-104">Or you may get the error: "There was a problem sending the command to the program."</span></span> <span data-ttu-id="7c636-105">Dafür gibt es viele Ursachen, aber die beiden gängigsten Lösungen sind:</span><span class="sxs-lookup"><span data-stu-id="7c636-105">There are many causes for this, but the two most common solutions are:</span></span>

- <span data-ttu-id="7c636-106">Stellen Sie in Excel sicher, dass die Option DDE deaktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="7c636-106">From within Excel, ensure that the DDE option is unchecked.</span></span> <span data-ttu-id="7c636-107">Die Option kann gefunden werden, indem Sie eine neue Arbeitsmappe erstellen und dann **Datei > Optionen > auswählen.**</span><span class="sxs-lookup"><span data-stu-id="7c636-107">The option can be found by creating a new workbook and then choosing **File > Options > Advanced**.</span></span> <span data-ttu-id="7c636-108">Deaktivieren Sie **im Abschnitt Allgemein** die Option Andere Anwendungen ignorieren, die dynamic Data Exchange **(DDE) verwenden.**</span><span class="sxs-lookup"><span data-stu-id="7c636-108">In the **General** section, uncheck the **Ignore other applications that use Dynamic Data Exchange (DDE)**.</span></span>

- <span data-ttu-id="7c636-109">Führen Sie eine Onlinereparatur aus, um die Standardeinstellungen wiederherzustellen.</span><span class="sxs-lookup"><span data-stu-id="7c636-109">Run an Online Repair to restore default settings.</span></span> <span data-ttu-id="7c636-110">Klicken Sie auf die Schaltfläche Windows Start, und suchen Sie nach "Systemsteuerung".</span><span class="sxs-lookup"><span data-stu-id="7c636-110">Click the Windows Start button and search for "Control Panel."</span></span> <span data-ttu-id="7c636-111">Öffnen Sie **die Systemsteuerung,** und wechseln Sie zu **Programme > Programme und Features**.</span><span class="sxs-lookup"><span data-stu-id="7c636-111">Open the **Control Panel**, and go to **Programs > Programs and Features**.</span></span> <span data-ttu-id="7c636-112">Klicken Sie dann mit der **rechten maustaste Microsoft Office [Version]** und wählen **Sie Ändern > Onlinereparatur aus.**</span><span class="sxs-lookup"><span data-stu-id="7c636-112">Then right-click **Microsoft Office [Version]** and choose **Change > Online Repair**.</span></span>

<span data-ttu-id="7c636-113">Wenn keine dieser Lösungen funktioniert, finden Sie im Supportartikel eine vollständigere Lösungsliste, wenn sie beim Doppelklicken auf eine [Office-Datei nicht geöffnet werden kann.](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6)</span><span class="sxs-lookup"><span data-stu-id="7c636-113">If neither of these solutions work, a more complete list of solutions can be found in the support article, [Double-clicking an Office file fails to open it](https://support.office.com/article/Double-clicking-an-Office-file-fails-to-open-it-1e9c0ad9-34c8-4440-a42e-d30186b29ed6).</span></span>
