---
title: Automatische Bereinigung veralteter Geräte in Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1285"
- "6700008"
ms.openlocfilehash: 49a15132253c59189e343aeaa1c11d450b344896
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47715020"
---
# <a name="automatic-cleanup-of-stale-devices-in-intune"></a><span data-ttu-id="0c4bc-102">Automatische Bereinigung veralteter Geräte in Intune</span><span class="sxs-lookup"><span data-stu-id="0c4bc-102">Automatic cleanup of stale devices in Intune</span></span>

<span data-ttu-id="0c4bc-103">Intune erlaubt es dem Administrator, ein Zeitintervall zwischen 90 und 270 Tagen zu konfigurieren, nach dem veraltete Geräte aus dem Dienst entfernt werden.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-103">Intune allows the admin to configure a time interval between 90 and 270 days, after which stale devices are removed from the service.</span></span> <span data-ttu-id="0c4bc-104">Diese Einstellung gilt organisationsweit wird nach ihrer Aktivierung sofort wirksam.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-104">This setting is organization wide and once activated goes into effect immediately.</span></span> <span data-ttu-id="0c4bc-105">Alle Geräte, die über einen Zeitraum, der die Einstellung überschreitet, keinen Check-In beim Intune-Server durchgeführt haben, werden endgültig gelöscht.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-105">Any devices not checked into the Intune server for a period exceeding the setting are permanently deleted.</span></span>

<span data-ttu-id="0c4bc-106">**Hinweis**: Nur MDM-Geräteobjekte sind für diese Bereinigungsaktion berechtigt.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-106">**Note** Only MDM device objects are eligible for this cleanup action.</span></span> <span data-ttu-id="0c4bc-107">Reine EAS-Geräteobjekte sind davon ausgeschlossen.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-107">EAS only device objects are excluded.</span></span>

<span data-ttu-id="0c4bc-108">Weitere Informationen, wann ein Gerät für die Löschung berechtigt wird, basierend auf der Einstellung für die Gerätebereinigung und seinem „Zustand“:</span><span class="sxs-lookup"><span data-stu-id="0c4bc-108">For additional information on when a device becomes eligible for deletion based on the device clean-up setting and its "state":</span></span>

<span data-ttu-id="0c4bc-109">Einstellung: **Geräte nach Datum des letzten Check-Ins löschen: Ja (ein Wert (N), Angabe in Tagen)**</span><span class="sxs-lookup"><span data-stu-id="0c4bc-109">Setting: **Delete devices after last check-in date: Yes (some value (N) in days specified)**</span></span>

- <span data-ttu-id="0c4bc-110">Basierend auf dem in der Einstellung konfigurierten Wert (N) löscht der Intune-Dienst das Gerät innerhalb der angegebenen Tagen, nachdem es zuletzt erfolgreich eingecheckt wurde.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-110">Based on value (N) configured in the setting, the Intune service deletes the device in the specified days after it last successfully checks in.</span></span>

<span data-ttu-id="0c4bc-111">Einstellung: **Geräte nach Datum des letzten Check-Ins löschen: Nein**</span><span class="sxs-lookup"><span data-stu-id="0c4bc-111">Setting:  **Delete devices after last check-in date: No**</span></span>

- <span data-ttu-id="0c4bc-112">180 Tage nachdem das Gerätezertifikat abgelaufen ist und nicht verlängert wurde, wird das Gerät gelöscht.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-112">180 days after the device certificate expires and is not renewed, the device is deleted.</span></span>

<span data-ttu-id="0c4bc-113">**Hinweis**: In beiden Fällen muss das Gerät erfolgreich bei Intune registriert sein.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-113">**Note** In both cases, the device must be registered successfully in Intune.</span></span> <span data-ttu-id="0c4bc-114">Die Registrierung erfolgt während des ersten Check-Ins des Geräts beim Intune-Dienst.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-114">Registration occurs during the first device checkin with the Intune service.</span></span>

<span data-ttu-id="0c4bc-115">Wird ein Gerät erfolgreich bei Intune registriert, aber nicht Intune-registriert, wird das Gerät 270 Tage nach seiner Registrierung gelöscht.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-115">If a device enrolls successfully to Intune but does not become Intune registered, the device is deleted 270 days after enrollment.</span></span> <span data-ttu-id="0c4bc-116">(90 Tage, um das Gerät als „Aufgehoben“ zu markieren, und dann weitere 180 Tage, um den Datensatz zu löschen.)</span><span class="sxs-lookup"><span data-stu-id="0c4bc-116">(90 days to mark the device as revoked, and then another 180 days to delete the record.)</span></span>

<span data-ttu-id="0c4bc-117">Zurzeit gibt es in der Intune-Konsole keinen Mechanismus zum Festlegen des Ablaufdatums der Gerätezertifizierung für ein bestimmtes Gerät.</span><span class="sxs-lookup"><span data-stu-id="0c4bc-117">No mechanism exists currently in the Intune console to establish the expiration date of the device certification for any given device.</span></span>