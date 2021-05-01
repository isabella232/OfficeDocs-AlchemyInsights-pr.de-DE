---
title: Problembehandlung Import-Serviceauftrag steckt fest
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/27/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7907"
- "9003046"
ms.openlocfilehash: 987383037f843d347477c0becc859c663736a676
ms.sourcegitcommit: c977687a7dd03288a9ba396cf2a48ea384d72634
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/27/2021
ms.locfileid: "52059845"
---
# <a name="troubleshooting-import-service-job-stuck"></a><span data-ttu-id="343e7-102">Problembehandlung Import-Serviceauftrag steckt fest</span><span class="sxs-lookup"><span data-stu-id="343e7-102">Troubleshooting Import Service job stuck</span></span>

<span data-ttu-id="343e7-103">Wenn Sie Probleme mit steckengebliebenen oder fehlgeschlagenen Import-Service-Jobs haben, prüfen Sie und versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="343e7-103">If you are experiencing issues with Import service jobs stuck or failing, examine and try the following:</span></span>

- <span data-ttu-id="343e7-104">Überprüfen Sie die Größe der PST-Datei.</span><span class="sxs-lookup"><span data-stu-id="343e7-104">Review the size of of the PST file.</span></span> <span data-ttu-id="343e7-105">Die maximal empfohlene Größe einer PST-Datei für den Import beträgt 20 GB.</span><span class="sxs-lookup"><span data-stu-id="343e7-105">The maximum recommended size of a PST file for import is 20GB.</span></span>

- <span data-ttu-id="343e7-106">Wenn Sie vermuten, dass Elemente aufgrund einer Beschädigung übersprungen wurden, führen Sie Scanpst.exe aus, um Fehler in PST-Dateien zu diagnostizieren und zu beheben.</span><span class="sxs-lookup"><span data-stu-id="343e7-106">If you suspect skipped items due to corruption, run Scanpst.exe to diagnose and fix errors in PST files.</span></span>

- <span data-ttu-id="343e7-107">Wenn Sie während des Imports die Fehlermeldung "MapiExceptionShutoffQuotaExceeded" sehen, stellen Sie sicher, dass das Zielpostfach genügend Kapazität hat, um die gewünschten PST-Dateien zu importieren.</span><span class="sxs-lookup"><span data-stu-id="343e7-107">If you see a "MapiExceptionShutoffQuotaExceeded" error during import, make sure the target mailbox has sufficient capacity to import the desired PST files.</span></span>

<span data-ttu-id="343e7-108">Weitere Informationen zur Problembehandlung bei PST-Importaufträgen finden Sie unter [Behebung von Problemen mit PST-Importaufträgen](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span><span class="sxs-lookup"><span data-stu-id="343e7-108">For more information on troubleshooting PST import job issues, see [Troubleshoot issues with PST import jobs](https://docs.microsoft.com/office365/troubleshoot/pst-import-service/issues-with-pst-import-job).</span></span>

<span data-ttu-id="343e7-109">Informationen darüber, wie Probleme beim Importieren von PST-Dateien in Outlook behoben werden können, finden Sie unter [Probleme beim Importieren einer Outlook-.pst-Datei beheben (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span><span class="sxs-lookup"><span data-stu-id="343e7-109">For information about how to fix issues when importing PSTs into Outlook, see [Fix problems importing an Outlook .pst file (microsoft.com)](https://support.microsoft.com/topic/fix-problems-importing-an-outlook-pst-file-2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e?ui=en-us&rs=en-us&ad=us).</span></span>