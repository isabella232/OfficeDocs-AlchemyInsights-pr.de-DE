---
title: Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"
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
- "9000171"
- "1712"
ms.openlocfilehash: 498c2ec78bc9f4a7bc7d77d12b488be2cf0bf79a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47666977"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="5d319-102">Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"</span><span class="sxs-lookup"><span data-stu-id="5d319-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="5d319-103">Der von Intune gemeldete App-Installationsfehler "Die Anwendung wurde nicht erkannt" nach erfolgreichem Abschluss der Installation kann auf allen wichtigen Betriebssystemplattformen (Windows, IOS und Android) auftreten.</span><span class="sxs-lookup"><span data-stu-id="5d319-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="5d319-104">Zu den häufigsten Szenarien, die diesen Fehler generieren, gehören:</span><span class="sxs-lookup"><span data-stu-id="5d319-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="5d319-105">Die App wurde nach der ersten Bereitstellung außerhalb von Intune (über den App Store eines Drittanbieters) aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="5d319-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="5d319-106">Einige Anwendungen wie Google Chrome können beispielsweise automatische Updates durchführen.</span><span class="sxs-lookup"><span data-stu-id="5d319-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="5d319-107">Ein Benutzer hat die App nach der Erstinstallation deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="5d319-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="5d319-108">Um dieses Problem zu vermeiden, untersuchen Sie zuerst die betroffenen Geräte, um das Szenario zu ermitteln, in dem der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="5d319-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="5d319-109">Wenn die App außerhalb von Intune aktualisiert wurde, kann die App-Bereitstellung so festgelegt werden, dass diese Anwendungsversion ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="5d319-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="5d319-110">Legen Sie dazu unter **App-Konfiguration > App-Informationen** die Option **App-Version ignorieren** auf **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="5d319-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="5d319-111">Bei der Ausrichtung auf den Kunden kann es sinnvoll sein, die Anwendung als "Erforderlich" bereitzustellen, um sicherzustellen, dass die neueste Version bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="5d319-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="5d319-112">Alternativ können Sie auf der iOS-Plattform die mit dem Apple-Volumenlizenzprogramm verknüpfte **AutoUpdate**-Funktionalität verwenden, die so konfiguriert werden kann, dass automatisch eine Aktualisierung auf neue Anwendungsversionen durchgeführt wird, sobald diese verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="5d319-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="5d319-113">Weitere Informationen zur Behandlung von Problemen bei der Installation von Apps finden Sie unter [Problembehandlung bei der App-Installation](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="5d319-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
