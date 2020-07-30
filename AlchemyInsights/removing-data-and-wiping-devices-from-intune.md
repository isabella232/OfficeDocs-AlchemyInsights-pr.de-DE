---
title: Entfernen von Daten und Zurücksetzen des Geräts aus Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "45434605"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="e8b83-102">Entfernen von Daten und Zurücksetzen des Geräts aus Intune</span><span class="sxs-lookup"><span data-stu-id="e8b83-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="e8b83-103">Die Aktionen "Gerät zurücksetzen" und "Gerät abkoppeln" können verwendet werden, um von Intune verwaltete Unternehmensdaten zu entfernen oder eine Zurücksetzung auf Werkseinstellungen durchzuführen und das Gerät auf seine Standardeinstellungen zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="e8b83-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="e8b83-104">Melden Sie sich bei der Microsoft 365-Geräteverwaltung an, und navigieren Sie zu **Geräte** > **Alle Geräte**.</span><span class="sxs-lookup"><span data-stu-id="e8b83-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="e8b83-105">Wählen Sie das Gerät aus, das Sie zurücksetzen möchten.</span><span class="sxs-lookup"><span data-stu-id="e8b83-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="e8b83-106">Wählen Sie die Art der Remotezurücksetzung aus, die Sie durchführen möchten.</span><span class="sxs-lookup"><span data-stu-id="e8b83-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="e8b83-107">Durch das Abkoppeln werden nur organisatorische Informationen gelöscht, während eine vollständige Zurücksetzung das Gerät auf die Werkseinstellungen zurücksetzt.</span><span class="sxs-lookup"><span data-stu-id="e8b83-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="e8b83-108">Wählen Sie zum Bestätigen **Ja** aus.</span><span class="sxs-lookup"><span data-stu-id="e8b83-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="e8b83-109">Bis die Zurücksetzung abgeschlossen ist, wird als Status der Geräteaktion "Abkoppeln ausstehend" angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e8b83-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="e8b83-110">Nachdem der Vorgang abgeschlossen ist, wird das mobile Gerät nicht mehr in der Liste der verwalteten Geräte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="e8b83-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="e8b83-111">**Hinweis** Unternehmensdaten können nicht von Geräten entfernt werden, die mit Azure AD VERBUNDEN sind.</span><span class="sxs-lookup"><span data-stu-id="e8b83-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="e8b83-112">Vollständige Informationen zu den Auswirkungen der Aktionen "Abkoppeln" und "Zurücksetzen", beispielsweise, was aufbewahrt und was gelöscht wird, finden Sie unter [Entfernen von Geräten durch Zurücksetzen, Abkoppeln oder manuelles Aufheben der Registrierung des Geräts](https://docs.microsoft.com/intune/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="e8b83-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="e8b83-113">Informationen dazu, wie Sie alle Daten von einem macOS-Gerät löschen, finden Sie unter [Löschen aller Daten von einem macOS-Gerät](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="e8b83-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>