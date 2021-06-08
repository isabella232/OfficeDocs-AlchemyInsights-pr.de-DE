---
title: Office kann nicht aktiviert werden
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798679"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="4c4a7-102">Office kann nicht aktiviert werden</span><span class="sxs-lookup"><span data-stu-id="4c4a7-102">Unable to activate Office</span></span>

<span data-ttu-id="4c4a7-103">**Hinweis**: Wenn Sie eine ältere Version von Windows verwenden (z. B. Windows 7), stellen Sie sicher, dass TLS 1.2 als Standard aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="4c4a7-104">Weitere Informationen finden Sie unter [Update zum Aktivieren von TLS 1.1 und TLS 1.2 als sichere Standardprotokolle in WinHTTP unter Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="4c4a7-105">Überprüfen Sie, ob Ihr Abonnementstatus abgelaufen ist.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="4c4a7-106">Stellen Sie sicher, dass Sie über ein Abonnement verfügen, das Clientlizenzen zulässt, z. B. Office 365 Business oder Business Premium, und [dass dem Benutzer eine Lizenz zugewiesen wurde](/microsoft-365/admin/manage/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="4c4a7-107">Stellen Sie sicher, dass sich der Benutzer bei Office mit dem gleichen Konto anmeldet, dem die Lizenz zugewiesen wurde.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="4c4a7-108">Auf der Seite [Office 365 Service Health](/office365/enterprise/view-service-health) werden mögliche bekannte Probleme mit dem Dienst angezeigt.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="4c4a7-p102">Überprüfen Sie Ihre Firewall-, Antivirensoftware- und Proxyeinstellungen, um sich zu vergewissern, dass sie nicht den Zugriff auf das Internet für Microsoft 365-Apps blockieren. Weitere Informationen finden Sie unter [Office 365-URLs und IP-Adressbereiche](/office365/enterprise/urls-and-ip-address-ranges "Office 365-URLs und -IP-Adressbereiche").</span><span class="sxs-lookup"><span data-stu-id="4c4a7-p102">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet. Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="4c4a7-111">**Tipp** Auf Windows-Computern können wir mehrere häufige Probleme bei der Anmeldung bei Office für Sie diagnostizieren und automatisch beheben.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="4c4a7-112">Laden Sie den **[Microsoft Support- und Wiederherstellungs-Assistent](https://aka.ms/SaRA-OfficeSignInScenario)** herunter.</span><span class="sxs-lookup"><span data-stu-id="4c4a7-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="4c4a7-113">Ergreifen Sie die folgenden Maßnahmen zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="4c4a7-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="4c4a7-114">Öffnen Sie eine Office-App, und [melden Sie sich von vorhandenen Benutzerkonten ab](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="4c4a7-115">[Entfernen Sie die Office-Lizenz](/microsoft-365/admin/manage/remove-licenses-from-users), und [weisen Sie sie neu zu](/microsoft-365/admin/manage/assign-licenses-to-users), und [melden Sie sich dann unter Verwendung des betroffenen Benutzerkontos bei Office an](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="4c4a7-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="4c4a7-116">Ausführen der [Aktivierungsproblembehandlung](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="4c4a7-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="4c4a7-117">Zurücksetzen des Office-Aktivierungsstatus</span><span class="sxs-lookup"><span data-stu-id="4c4a7-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Zurücksetzen des Office-Aktivierungsstatus")
- [<span data-ttu-id="4c4a7-118">Ausführen einer Onlinereparatur von Office</span><span class="sxs-lookup"><span data-stu-id="4c4a7-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="4c4a7-119">Zusätzliche Lösungen zur Problembehandlung finden Sie unter:</span><span class="sxs-lookup"><span data-stu-id="4c4a7-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="4c4a7-120">Fehler "Nicht lizenziertes Produkt" und Aktivierungsfehler in Office</span><span class="sxs-lookup"><span data-stu-id="4c4a7-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="4c4a7-121">Fehler "Leider können wir keine Verbindung mit Ihrem Konto herstellen. Versuchen Sie es bitte später erneut" bei der Aktivierung von Office</span><span class="sxs-lookup"><span data-stu-id="4c4a7-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)