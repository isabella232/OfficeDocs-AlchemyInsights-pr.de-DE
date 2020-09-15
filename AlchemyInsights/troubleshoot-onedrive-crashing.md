---
title: Fehlerbehandlung bei OneDrive-Abstürzen
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003084"
- "5885"
ms.openlocfilehash: 1155d370911b28bbb1ba83a15eace66d1daea28f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664997"
---
# <a name="troubleshoot-onedrive-crashes"></a><span data-ttu-id="ac469-102">Fehlerbehandlung bei OneDrive-Abstürzen</span><span class="sxs-lookup"><span data-stu-id="ac469-102">Troubleshoot OneDrive crashes</span></span>

<span data-ttu-id="ac469-103">Wenn OneDrive wiederholt abstürzt, versuchen Sie die folgenden Schritte zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="ac469-103">If OneDrive repeatedly crashes, try these troubleshooting steps:</span></span>

<span data-ttu-id="ac469-104">**Stellen Sie sicher, dass die Registrierungsschlüssel nicht festgelegt sind:**</span><span class="sxs-lookup"><span data-stu-id="ac469-104">**Ensure registry keys aren’t set:**</span></span>

1. <span data-ttu-id="ac469-105">Navigieren Sie mithilfe des Registrierungs-Editors zu HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span><span class="sxs-lookup"><span data-stu-id="ac469-105">Using Registry Editor, navigate to HKEY_LOCAL_MACHINE\SOFTWARE\Policies\Microsoft\OneDrive</span></span>
2. <span data-ttu-id="ac469-106">Wenn „DisableFileSyncNGSC“ vorhanden und auf „1“ festgelegt ist, öffnen Sie den Schlüssel und ändern Sie den Wert auf „0“.</span><span class="sxs-lookup"><span data-stu-id="ac469-106">If DisableFileSyncNGSC is present and set to 1, open the key and change the value to 0.</span></span>
3. <span data-ttu-id="ac469-107">Starten Sie OneDrive manuell, indem Sie zu „Start“ wechseln.</span><span class="sxs-lookup"><span data-stu-id="ac469-107">Manually launch OneDrive by going to Start</span></span> ![Drücken Sie die WINDOWS-TASTE,](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="ac469-109">geben Sie im Suchfeld den Begriff OneDrive ein und klicken Sie dann auf die OneDrive Desktop-App.</span><span class="sxs-lookup"><span data-stu-id="ac469-109">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="ac469-110">**OneDrive zurücksetzen:**</span><span class="sxs-lookup"><span data-stu-id="ac469-110">**Reset OneDrive:**</span></span>

<span data-ttu-id="ac469-111">Hinweise:</span><span class="sxs-lookup"><span data-stu-id="ac469-111">Notes:</span></span>

- <span data-ttu-id="ac469-112">Beim Zurücksetzen von OneDrive werden alle Ihre bestehenden Synchronisierungsverbindungen (einschließlich – sofern eingerichtet – Ihr persönliches OneDrive) getrennt.</span><span class="sxs-lookup"><span data-stu-id="ac469-112">Resetting OneDrive disconnects all your existing sync connections (including your personal OneDrive if set up).</span></span>
- <span data-ttu-id="ac469-113">Wenn Sie OneDrive auf Ihrem Computer zurücksetzen, gehen keine Dateien oder Daten verloren.</span><span class="sxs-lookup"><span data-stu-id="ac469-113">You won't lose files or data by resetting OneDrive on your computer.</span></span>

<span data-ttu-id="ac469-114">**Zurücksetzen von OneDrive:**</span><span class="sxs-lookup"><span data-stu-id="ac469-114">**To reset OneDrive:**</span></span>

1. <span data-ttu-id="ac469-115">Öffnen Sie ein Dialogfeld „Ausführen“, indem Sie die WINDOWS-TASTE und R drücken.</span><span class="sxs-lookup"><span data-stu-id="ac469-115">Open a Run dialog by pressing Windows key    and R.</span></span>
2. <span data-ttu-id="ac469-116">Geben Sie „%localappdata%\Microsoft\OneDrive\onedrive.exe /reset“ ein und klicken Sie auf OK.</span><span class="sxs-lookup"><span data-stu-id="ac469-116">Type %localappdata%\Microsoft\OneDrive\onedrive.exe /reset and press OK.</span></span> <span data-ttu-id="ac469-117">Möglicherweise wird kurz ein Befehlsfenster eingeblendet.</span><span class="sxs-lookup"><span data-stu-id="ac469-117">A Command window may appear briefly.</span></span>
3. <span data-ttu-id="ac469-118">Starten Sie OneDrive manuell, indem Sie zu „Start“ wechseln.</span><span class="sxs-lookup"><span data-stu-id="ac469-118">Manually launch OneDrive by going to Start</span></span> ![Drücken Sie die WINDOWS-TASTE,](data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABEAAAAOCAYAAADJ7fe0AAAAAXNSR0IArs4c6QAAAARnQU1BAACxjwv8YQUAAAAJcEhZcwAADsQAAA7EAZUrDhsAAADxSURBVDhPY/wPBAx4wR+Gd6/fM7x9/ZTh9ZuXDGdPnWE4tH0rw/UHDxlaVp9kCDCSYWABKfv35wfD+/cfGV4+fcLw5uVjhlOXzzFsX/qWYebmZAZPWWOGO2DD8ACQS9Y3e4Bcg4Y9/t94fPa/CoY4Aq8/+xik/T8TkEMxGDyGgANWwSqeobvbGSyAADIM3BwCDKXd3QyfoCLoQEGAA0xTxSWjsYMJwLHjkruU4UXSJ4YnT54x3Dh/luHmjfMMmw9wMjCDlRAGBDPgjy8fGT5//8rw9P4Thge3zzNcvXmDYevmfQzXb1xlmH/0ATADyjAAAKdWkD3ZSwNeAAAAAElFTkSuQmCC)<span data-ttu-id="ac469-120">geben Sie im Suchfeld den Begriff OneDrive ein und klicken Sie dann auf die OneDrive Desktop-App.</span><span class="sxs-lookup"><span data-stu-id="ac469-120">, type OneDrive in the search box, and then click on the OneDrive desktop app.</span></span>

<span data-ttu-id="ac469-121">Hinweise:</span><span class="sxs-lookup"><span data-stu-id="ac469-121">Notes:</span></span>

- <span data-ttu-id="ac469-122">Wenn Sie vor dem Zurücksetzen ausgewählt hatten, dass nur einige Ordner synchronisiert werden sollen, müssen Sie dies nach Abschluss der Synchronisierung erneut tun.</span><span class="sxs-lookup"><span data-stu-id="ac469-122">If you had chosen to sync only some folders before the reset, you will need to do that again once sync has completed.</span></span> <span data-ttu-id="ac469-123">Weitere Informationen finden Sie unter  [Auswählen der OneDrive-Ordner, die mit Ihrem Computer synchronisiert werden sollen](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) .</span><span class="sxs-lookup"><span data-stu-id="ac469-123">Read [Choose which OneDrive folders to sync to your computer](https://support.office.com/article/98b8b011-8b94-419b-aa95-a14ff2415e85) for more information.</span></span>
- <span data-ttu-id="ac469-124">Sie müssen dies für Ihr persönliches OneDrive und für OneDrive for Business ausführen.</span><span class="sxs-lookup"><span data-stu-id="ac469-124">You will need to complete this for your personal OneDrive and OneDrive for Business.</span></span>