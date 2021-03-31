---
title: Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: f51a455ea15b7bd92f548f2c1717be9888b43d07
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426840"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-domain-joined-device"></a><span data-ttu-id="beda5-102">Microsoft Edge als Standardbrowser auf einem domänenverbundenen Gerät festlegen</span><span class="sxs-lookup"><span data-stu-id="beda5-102">Set Microsoft Edge as the default browser on a domain-joined device</span></span>

<span data-ttu-id="beda5-103">Legen Sie Microsoft Edge als Standardbrowser fest:</span><span class="sxs-lookup"><span data-stu-id="beda5-103">Set Microsoft Edge as the default browser:</span></span> 

1. <span data-ttu-id="beda5-104">[Erstellen Sie eine Konfigurationsdatei für Standardverknüpfungen](https://go.microsoft.com/fwlink/?linkid=2132437) und speichern Sie sie lokal oder auf einer Netzwerkfreigabe.</span><span class="sxs-lookup"><span data-stu-id="beda5-104">[Create a default associations configuration file](https://go.microsoft.com/fwlink/?linkid=2132437) and store it locally or on a network share.</span></span>

1. <span data-ttu-id="beda5-105">Öffnen Sie den Gruppenrichtlinien-Editor und gehen Sie dann zu **Computerkonfiguration** > **Administrative Vorlagen** > **Windows-Komponenten** > **Datei-Explorer**.</span><span class="sxs-lookup"><span data-stu-id="beda5-105">Open the Group Policy editor, and then go to **Computer Configuration** > **Administrative Templates** > **Windows Components** > **File Explorer**.</span></span>

1. <span data-ttu-id="beda5-106">Wählen Sie **Konfigurationsdatei für Standardverknüpfungen festlegen**.</span><span class="sxs-lookup"><span data-stu-id="beda5-106">Select **Set a default associations configuration file**.</span></span>

1. <span data-ttu-id="beda5-107">Wählen Sie **Richtlinieneinstellung**, und wählen Sie dann **Aktiviert**.</span><span class="sxs-lookup"><span data-stu-id="beda5-107">Select **Policy setting**, and then select **Enabled**.</span></span>

1. <span data-ttu-id="beda5-108">Geben Sie unter **Optionen** den Speicherort der Konfigurationsdatei für die Standardverknüpfungen ein und wählen Sie dann **OK**.</span><span class="sxs-lookup"><span data-stu-id="beda5-108">Under **Options**, enter the location of your default associations configuration file, and then select **OK**.</span></span>
