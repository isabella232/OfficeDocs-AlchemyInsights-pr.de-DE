---
title: Senden von benutzerdefinierten Benachrichtigungen mit InTune
ms.author: brenduns
author: brenduns
manager: dougeby
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000679"
- "2565"
ms.openlocfilehash: 2e5e2e2f24c46d3db4f08862dcc80934937f6f51
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720645"
---
# <a name="how-to-send-custom-notifications-to-the-users-of-managed-ios-and-android-devices"></a><span data-ttu-id="f1d82-102">Vorgehensweise Senden von benutzerdefinierten Benachrichtigungen an die Benutzer von verwalteten IOS-und Android-Geräten</span><span class="sxs-lookup"><span data-stu-id="f1d82-102">How to send custom notifications to the users of managed iOS and Android devices</span></span>

<span data-ttu-id="f1d82-103">Benutzerdefinierte Benachrichtigungen für InTune werden von der Unternehmens Portal-App auf dem Gerät eines Benutzers verarbeitet.</span><span class="sxs-lookup"><span data-stu-id="f1d82-103">Custom notifications for Intune are processed by the Company Portal app on a user’s device.</span></span> <span data-ttu-id="f1d82-104">Die App erstellt dann die Push-Benachrichtigung auf dem Gerät.</span><span class="sxs-lookup"><span data-stu-id="f1d82-104">The app then creates the push notification on that device.</span></span>

<span data-ttu-id="f1d82-105">Im folgenden sind Geräte Voraussetzungen für die Unterstützung des Empfangs von benutzerdefinierten Benachrichtigungen und für die anschließende Erstellung der Push-Benachrichtigung durch die APP beschrieben:</span><span class="sxs-lookup"><span data-stu-id="f1d82-105">The following are device prerequisites to support receipt of custom notifications, and for the app to then create the push notification:</span></span>

- <span data-ttu-id="f1d82-106">Auf dem Gerät muss die Unternehmens Portal-App installiert sein.</span><span class="sxs-lookup"><span data-stu-id="f1d82-106">The device must have the Company Portal app installed.</span></span>  

- <span data-ttu-id="f1d82-107">Das Gerät muss zulassen, dass die Unternehmens Portal-App Push-Benachrichtigungen sendet.</span><span class="sxs-lookup"><span data-stu-id="f1d82-107">The device must allow the Company Portal app to send push notifications.</span></span> <span data-ttu-id="f1d82-108">Wenn die APP installiert oder aktualisiert wird, wird der Benutzer aufgefordert, Benachrichtigungen zu erlauben.</span><span class="sxs-lookup"><span data-stu-id="f1d82-108">When the app is installed or updated, it will prompt the user to permit notifications.</span></span>

- <span data-ttu-id="f1d82-109">Auf Android-Geräten muss Google Play Services installiert sein.</span><span class="sxs-lookup"><span data-stu-id="f1d82-109">Android devices must have Google Play Services installed.</span></span>

- <span data-ttu-id="f1d82-110">Das Gerät muss mit InTune registriert sein.</span><span class="sxs-lookup"><span data-stu-id="f1d82-110">The device must be enrolled with Intune.</span></span>

<span data-ttu-id="f1d82-111">Weitere Informationen, einschließlich der Vorgehensweise zum Senden einer Nachricht, finden Sie in der [Feature-Dokumentation](https://docs.microsoft.com/intune/custom-notifications).</span><span class="sxs-lookup"><span data-stu-id="f1d82-111">For more information including how to send a message, see the [feature documentation](https://docs.microsoft.com/intune/custom-notifications).</span></span>
