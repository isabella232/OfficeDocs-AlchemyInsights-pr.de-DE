---
title: Verwenden von E-Mail-Profilen mit Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1559"
- "9000076"
ms.openlocfilehash: 5aae83a0ab26c2bd59fddd2ad64d1c461d29f0f7
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 07/28/2020
ms.locfileid: "46505217"
---
# <a name="using-email-profiles-with-intune"></a><span data-ttu-id="41f61-102">Verwenden von E-Mail-Profilen mit Intune</span><span class="sxs-lookup"><span data-stu-id="41f61-102">Using email profiles with Intune</span></span>

<span data-ttu-id="41f61-103">Intune kann verwendet werden, um E-Mail-Profile für den nativen (integrierten) E-Mail-Client auf mehreren Geräteplattformen zu erstellen und bereitzustellen.</span><span class="sxs-lookup"><span data-stu-id="41f61-103">Intune can be used to create and deploy email profiles for the native (built-in) email client on multiple device platforms.</span></span>

<span data-ttu-id="41f61-104">Informationen über einige der Einschränkungen, die mit E-Mail-Profilen verbunden sind, einschließlich der Verarbeitung vorhandener Profile und der Entfernung von E-Mail-Profilen, finden Sie unter [Hinzufügen von E-Mail-Einstellungen für Geräte mit Intune](https://docs.microsoft.com/intune/email-settings-configure).</span><span class="sxs-lookup"><span data-stu-id="41f61-104">For info about some of the restrictions associated with email profiles, including how the presence of existing profiles are handled and how to remove email profiles, see [Add email settings to devices using Intune](https://docs.microsoft.com/intune/email-settings-configure).</span></span>

<span data-ttu-id="41f61-105">Weitere Informationen zum Erstellen von E-Mail-Profilen für jede Geräteplattform finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="41f61-105">For more info about how to create email profiles for each device platform, see:</span></span>

[<span data-ttu-id="41f61-106">Android-Geräteeinstellungen zum Konfigurieren von E-Mail, Authentifizierung und Synchronisierung in Intune</span><span class="sxs-lookup"><span data-stu-id="41f61-106">Android device settings to configure email, authentication, and synchronization in Intune</span></span>](https://docs.microsoft.com/intune/email-settings-android)  
[<span data-ttu-id="41f61-107">Hinzufügen von E-Mail-Einstellungen für iOS- und iPadOS-Geräte in Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="41f61-107">Add e-mail settings for iOS and iPadOS devices in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-ios)  
[<span data-ttu-id="41f61-108">E-Mail-Profileinstellungen in Microsoft Intune für Windows Phone 8.1-Geräte</span><span class="sxs-lookup"><span data-stu-id="41f61-108">Email profile settings in Microsoft Intune for devices running Windows Phone 8.1</span></span>](https://docs.microsoft.com/intune/email-settings-windows-phone-8-1)  
[<span data-ttu-id="41f61-109">E-Mail-Profileinstellungen für Geräte in Microsoft Intune, die unter Windows 10 ausgeführt werden</span><span class="sxs-lookup"><span data-stu-id="41f61-109">Email profile settings for devices running Windows 10 in Microsoft Intune</span></span>](https://docs.microsoft.com/intune/email-settings-windows-10)

<span data-ttu-id="41f61-110">**Häufig auftretendes Synchronisierungsproblem**</span><span class="sxs-lookup"><span data-stu-id="41f61-110">**Common syncing issue**</span></span>

<span data-ttu-id="41f61-111">**Ein KNOX unter Android-E-Mail-Profil verhindert, dass die Kontakte, Kalender und Aufgaben des Benutzers mit den Geräten des Benutzers synchronisiert werden.**</span><span class="sxs-lookup"><span data-stu-id="41f61-111">**A KNOX on Android email profile prevents user Contacts, Calendar, and Tasks, from being sync'd to user devices.**</span></span>

<span data-ttu-id="41f61-112">Das KNOX unter Android KNOX-E-Mail-Profil bietet dem Administrator die Möglichkeit zu entscheiden, welche Inhaltstypen mit dem Gerät synchronisiert werden, indem die gewünschten Inhaltstypen auf "Aktiviert" festgelegt werden.</span><span class="sxs-lookup"><span data-stu-id="41f61-112">The KNOX on Android KNOX email profile offers the admin the option to decide which content types are sync'd to the device by setting each to enabled.</span></span>

<span data-ttu-id="41f61-113">Wenn die Einstellung für einen der Inhaltstypen auf **Nicht konfiguriert** (Standardeinstellung) festgelegt ist, wird dieser Inhaltstyp nicht automatisch synchronisiert.</span><span class="sxs-lookup"><span data-stu-id="41f61-113">If the setting for any of the content types is set to **Not configured** (the default), that content type is not sync'd automatically.</span></span> <span data-ttu-id="41f61-114">Ein Benutzer könnte den gewünschten Inhaltstyp direkt auf dem Gerät manuell aktivieren, aber diese Konfiguration wird durch die Intune-Richtlinieneinstellung außer Kraft gesetzt, und die Synchronisierung wird für diesen Inhaltstyp beendet.</span><span class="sxs-lookup"><span data-stu-id="41f61-114">A user might enable the content type they want directly on the device manually, but that configuration is overwritten by the Intune policy setting, and the sync stops for that content type.</span></span>

