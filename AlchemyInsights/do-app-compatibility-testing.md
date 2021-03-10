---
title: Durchführen von App-Kompatibilitätstests
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9138"
- "9005291"
ms.openlocfilehash: 9a6a9ea3587a851ecf842588ab73421590ce2431
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50530009"
---
# <a name="do-app-compatibility-testing"></a><span data-ttu-id="fbd5e-102">Durchführen von App-Kompatibilitätstests</span><span class="sxs-lookup"><span data-stu-id="fbd5e-102">Do app compatibility testing</span></span>

<span data-ttu-id="fbd5e-103">Die Anwendungskompatibilität für Microsoft Edge ist extrem hoch.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-103">Application compatibility for Microsoft Edge is extremely high.</span></span> <span data-ttu-id="fbd5e-104">Sie ist tatsächlich so hoch, dass Microsoft diesbezüglich die folgenden Versprechen geben kann:</span><span class="sxs-lookup"><span data-stu-id="fbd5e-104">In fact, it's so high that Microsoft provides the following compatibility promises:</span></span>
- <span data-ttu-id="fbd5e-105">Wenn etwas in Microsoft Edge 45 und früheren Versionen verwendet werden kann, funktioniert es auch mit Microsoft Edge 77 und neueren Versionen.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-105">If it works on Microsoft Edge 45 and earlier versions, it will work on Microsoft Edge 77 and later versions.</span></span>
- <span data-ttu-id="fbd5e-106">Wenn es im Internet Explorer funktioniert, funktioniert es auch in Microsoft Edge im Internet Explorer-Modus.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-106">If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.</span></span>
- <span data-ttu-id="fbd5e-107">Wenn es in Google Chrome funktioniert, funktioniert es auch in Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-107">If it works on Google Chrome, it will work on Microsoft Edge.</span></span>

<span data-ttu-id="fbd5e-108">Wenn Sie über eine Anwendung verfügen, bei der diese Versprechen nicht erfüllt werden, stehen wir zu dem Versprechen, das zu beheben, durch [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span><span class="sxs-lookup"><span data-stu-id="fbd5e-108">If you have an application where we don't meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/fasttrack/microsoft-365/app-assure).</span></span>

<span data-ttu-id="fbd5e-109">Trotz dieser Versprechen wissen wir, dass viele Organisationen einige Anwendungen auf Kompatibilitäts- oder Risikomanagementgründen überprüfen müssen.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-109">Despite this promise, we know that many organizations must validate some applications for compliance or risk-management reasons.</span></span> <span data-ttu-id="fbd5e-110">Obwohl wir davon ausgehen, dass dies sehr einfach ist, ist es wichtig, bei App-Tests organisiert und rigoros vorzugehen.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-110">Even though we expect this to be very straightforward, it's important to be organized and rigorous in app testing.</span></span>

<span data-ttu-id="fbd5e-111">Es gibt zwei Möglichkeiten zum Testen der App-Kompatibilität:</span><span class="sxs-lookup"><span data-stu-id="fbd5e-111">There are two ways to do app compatibility testing:</span></span>

- <span data-ttu-id="fbd5e-112">**Tests in Testumgebungen**: Die Anwendungen werden in einer streng kontrollierten Umgebung mit bestimmten Konfigurationen getestet.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-112">**Lab testing**: Applications are tested in a tightly controlled environment with specific configurations.</span></span>
- <span data-ttu-id="fbd5e-113">**Pilottests**: Die Anwendungen werden von einer begrenzten Anzahl von Benutzern in ihrer täglichen Arbeitsumgebung auf ihren eigenen Geräten getestet.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-113">**Pilot testing**: Applications are tested by a limited number of users in their daily work environment using their own devices.</span></span>

<span data-ttu-id="fbd5e-114">Wählen Sie die Methode aus, die für die jeweilige App am besten geeignet ist, und führen Sie den Test vor einer Einführung für die gesamte Organisation durch.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-114">Choose the method that is most appropriate for each app and do the testing prior to a launch to the entire organization.</span></span>

<span data-ttu-id="fbd5e-115">Nachdem Sie sich vergewissert haben, dass Ihre Apps kompatibel sind, können Sie Microsoft Edge für eine Pilotgruppe bereitstellen.</span><span class="sxs-lookup"><span data-stu-id="fbd5e-115">Once you've ensured that your apps are compatible, you're ready to deploy Microsoft Edge to a pilot group.</span></span>
