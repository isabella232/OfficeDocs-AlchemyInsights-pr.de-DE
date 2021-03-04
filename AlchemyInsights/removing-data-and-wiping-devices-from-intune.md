---
title: Entfernen von Daten und Zurücksetzen des Geräts aus Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416312"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="b8008-102">Entfernen von Daten und Zurücksetzen des Geräts aus Intune</span><span class="sxs-lookup"><span data-stu-id="b8008-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="b8008-103">Die Aktionen "Gerät zurücksetzen" und "Gerät abkoppeln" können verwendet werden, um von Intune verwaltete Unternehmensdaten zu entfernen oder eine Zurücksetzung auf Werkseinstellungen durchzuführen und das Gerät auf seine Standardeinstellungen zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="b8008-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="b8008-104">Melden Sie sich bei der Microsoft 365-Geräteverwaltung an, und navigieren Sie zu **Geräte** > **Alle Geräte**.</span><span class="sxs-lookup"><span data-stu-id="b8008-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="b8008-105">Wählen Sie das Gerät aus, das Sie zurücksetzen möchten.</span><span class="sxs-lookup"><span data-stu-id="b8008-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="b8008-106">Wählen Sie die Art der Remotezurücksetzung aus, die Sie durchführen möchten.</span><span class="sxs-lookup"><span data-stu-id="b8008-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="b8008-107">Durch das Abkoppeln werden nur organisatorische Informationen gelöscht, während eine vollständige Zurücksetzung das Gerät auf die Werkseinstellungen zurücksetzt.</span><span class="sxs-lookup"><span data-stu-id="b8008-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="b8008-108">Wählen Sie zum Bestätigen **Ja** aus.</span><span class="sxs-lookup"><span data-stu-id="b8008-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="b8008-109">Bis zum Löschen wird der Status der Geräteaktion als *Abkoppeln ausstehend* angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8008-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="b8008-110">Nach Abschluss der Aktion wird das mobile Gerät nicht mehr in der Liste der verwalteten Geräte angezeigt.</span><span class="sxs-lookup"><span data-stu-id="b8008-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="b8008-111">Unternehmensdaten können nicht von Geräten entfernt werden, die mit Azure AD verbunden sind.</span><span class="sxs-lookup"><span data-stu-id="b8008-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="b8008-112">Ausführliche Informationen zu den Auswirkungen der Aktionen "Abkoppeln" und "Zurücksetzen", einschließlich der beibehaltenen und gelöschten Aktionen, finden Sie in der folgenden Dokumentation:</span><span class="sxs-lookup"><span data-stu-id="b8008-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="b8008-113">[Entfernen Sie Geräte, indem Sie das Gerät zurücksetzen, abkoppeln oder manuell abmelden](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="b8008-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="b8008-114">So löschen Sie nur Unternehmensdaten aus von Intune verwalteten Apps</span><span class="sxs-lookup"><span data-stu-id="b8008-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="b8008-115">[Löschen allen Daten von einem MacOS-Gerät](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="b8008-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>