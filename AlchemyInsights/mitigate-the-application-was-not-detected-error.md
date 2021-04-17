---
title: Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 4e0599f9bdf2c7d16d009627f44b3691c2c250b7
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836350"
---
# <a name="mitigate-the-application-was-not-detected-error"></a><span data-ttu-id="52341-102">Beheben des Fehlers "Sie Anwendung wurde nicht erkannt"</span><span class="sxs-lookup"><span data-stu-id="52341-102">Mitigate "The application was not detected" error</span></span>

<span data-ttu-id="52341-103">Der von Intune gemeldete App-Installationsfehler "Die Anwendung wurde nicht erkannt" nach erfolgreichem Abschluss der Installation kann auf allen wichtigen Betriebssystemplattformen (Windows, IOS und Android) auftreten.</span><span class="sxs-lookup"><span data-stu-id="52341-103">The app installation error, “The application was not detected after installation completed successfully,” reported by Intune, may occur on all major OS platforms (Windows, iOS and Android).</span></span>

<span data-ttu-id="52341-104">Zu den häufigsten Szenarien, die diesen Fehler generieren, gehören:</span><span class="sxs-lookup"><span data-stu-id="52341-104">The most common scenarios that generate this error include:</span></span>

- <span data-ttu-id="52341-105">Die App wurde nach der ersten Bereitstellung außerhalb von Intune (über den App Store eines Drittanbieters) aktualisiert.</span><span class="sxs-lookup"><span data-stu-id="52341-105">The app has been updated outside of Intune (from a third-party app store) after the initial deployment.</span></span> <span data-ttu-id="52341-106">Einige Anwendungen wie Google Chrome können beispielsweise automatische Updates durchführen.</span><span class="sxs-lookup"><span data-stu-id="52341-106">For example some applications such as Google Chrome may perform auto updates.</span></span>
- <span data-ttu-id="52341-107">Ein Benutzer hat die App nach der Erstinstallation deinstalliert.</span><span class="sxs-lookup"><span data-stu-id="52341-107">A user has uninstalled the app after the initial install.</span></span>

<span data-ttu-id="52341-108">Um dieses Problem zu vermeiden, untersuchen Sie zuerst die betroffenen Geräte, um das Szenario zu ermitteln, in dem der Fehler aufgetreten ist.</span><span class="sxs-lookup"><span data-stu-id="52341-108">To mitigate this issue, first perform a review of the affected devices to determine the scenario in which the error occurs.</span></span>

- <span data-ttu-id="52341-109">Wenn die App außerhalb von Intune aktualisiert wurde, kann die App-Bereitstellung so festgelegt werden, dass diese Anwendungsversion ignoriert wird.</span><span class="sxs-lookup"><span data-stu-id="52341-109">If the app has been updated outside of Intune, the app deployment can be set to ignore the application version.</span></span> <span data-ttu-id="52341-110">Legen Sie dazu unter **App-Konfiguration > App-Informationen** die Option **App-Version ignorieren** auf **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="52341-110">To do so, under **App Configuration > App Information**, set **Ignore App** version to **Yes**.</span></span>
- <span data-ttu-id="52341-111">Bei der Ausrichtung auf den Kunden kann es sinnvoll sein, die Anwendung als "Erforderlich" bereitzustellen, um sicherzustellen, dass die neueste Version bereitgestellt wird.</span><span class="sxs-lookup"><span data-stu-id="52341-111">When targeting the client, it may be appropriate to deploy the application as “required,” and to ensure that the latest version is deployed.</span></span>
- <span data-ttu-id="52341-112">Alternativ können Sie auf der iOS-Plattform die mit dem Apple-Volumenlizenzprogramm verknüpfte **AutoUpdate**-Funktionalität verwenden, die so konfiguriert werden kann, dass automatisch eine Aktualisierung auf neue Anwendungsversionen durchgeführt wird, sobald diese verfügbar sind.</span><span class="sxs-lookup"><span data-stu-id="52341-112">Alternatively, on the iOS platform, it is possible to use the **autoupdate** functionality associated with the Apple Volume Purchase Program, which can be configured to automatically update to new application versions as they become available.</span></span>

<span data-ttu-id="52341-113">Weitere Informationen zur Behandlung von Problemen bei der Installation von Apps finden Sie unter [Problembehandlung bei der App-Installation](https://docs.microsoft.com/intune/troubleshoot-app-install).</span><span class="sxs-lookup"><span data-stu-id="52341-113">For more information about troubleshooting app installation issues, please see [Troubleshoot app installation issues](https://docs.microsoft.com/intune/troubleshoot-app-install).</span></span>
