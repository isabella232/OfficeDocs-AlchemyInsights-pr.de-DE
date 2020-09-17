---
title: Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten
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
- "9002931"
- "5612"
ms.openlocfilehash: 285933e607ac7e58256709f0c9cf2851250ce211
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806434"
---
# <a name="enable-embedding-legacy-dialogs-to-open-reports"></a><span data-ttu-id="7c5ea-102">Aktivieren der Einbettung von alten Dialogen zum Öffnen von Berichten</span><span class="sxs-lookup"><span data-stu-id="7c5ea-102">Enable embedding legacy dialogs to open reports</span></span>

<span data-ttu-id="7c5ea-103">**Symptom**</span><span class="sxs-lookup"><span data-stu-id="7c5ea-103">**Symptom**</span></span>

<span data-ttu-id="7c5ea-104">Benutzer können keine Berichte öffnen.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-104">Users are unable to open reports.</span></span> <span data-ttu-id="7c5ea-105">"Es ist ein Fehler aufgetreten.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-105">"Something has gone wrong.</span></span> <span data-ttu-id="7c5ea-106">Überprüfen Sie die technischen Details, um weitere Informationen zu erhalten."</span><span class="sxs-lookup"><span data-stu-id="7c5ea-106">Check technical details for more details."</span></span>

<span data-ttu-id="7c5ea-107">**Ursache**</span><span class="sxs-lookup"><span data-stu-id="7c5ea-107">**Cause**</span></span>

<span data-ttu-id="7c5ea-108">Berichte können nicht in UCI geladen werden, und der Fehler "Formularbeschreibung ist "null" oder nicht definiert" wird angezeigt.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-108">Reports are failing to load in UCI with the error, "Form descriptor is null or not defined."</span></span> <span data-ttu-id="7c5ea-109">Berichte in UCI erfordern immer noch alte Dialoge, daher muss im System des Kunden *allowlegacydialogsembedding* aktiviert sein.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-109">Reports in UCI still require legacy dialogs, so the customer's system needs to have *allowlegacydialogsembedding* enabled.</span></span>

<span data-ttu-id="7c5ea-110">**Lösung**</span><span class="sxs-lookup"><span data-stu-id="7c5ea-110">**Solution**</span></span>

1. <span data-ttu-id="7c5ea-111">Navigieren Sie zu **Einstellungen > Verwaltung > Systemeinstellungen > Registerkarte "Allgemein"**.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-111">Go to **Settings >Administration > System Settings > General tab**.</span></span>

2. <span data-ttu-id="7c5ea-112">Legen Sie "Einbettung bestimmter alter Dialoge in den Browserclient der einheitlichen Oberfläche aktivieren" auf **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="7c5ea-112">Set "Enable embedding of certain legacy dialogs in Unified Interface browser client" to **Yes**.</span></span>
