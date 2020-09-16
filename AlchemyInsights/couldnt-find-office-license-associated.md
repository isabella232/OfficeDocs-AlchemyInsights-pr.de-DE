---
title: Fixieren von Microsoft 365-apps konnten keine Office-Lizenzen finden. zugeordnete Nachricht
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747694"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a><span data-ttu-id="6e6e6-102">Beheben der Nachricht "Office-Lizenzen konnten nicht gefunden werden" für Microsoft 365-apps</span><span class="sxs-lookup"><span data-stu-id="6e6e6-102">Fixing the Microsoft 365 apps "Couldn't find office licenses associated" message</span></span>

<span data-ttu-id="6e6e6-103">Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="6e6e6-103">If you receive this message, try the following:</span></span>

1. <span data-ttu-id="6e6e6-104">Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Microsoft 365-apps nicht blockiert wird.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-104">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Internet access to Microsoft 365 apps.</span></span> <span data-ttu-id="6e6e6-105">Weitere Informationen finden Sie unter [Microsoft 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6e6e6-105">See [Microsoft 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>
2. <span data-ttu-id="6e6e6-106">Entfernen Sie [die Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) für den betroffenen Benutzer, und weisen Sie Sie neu zu.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-106">Remove and [reassign the Office license](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) for the affected user.</span></span> 
3. <span data-ttu-id="6e6e6-107">Öffnen Sie eine Office-App, und [melden Sie sich](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bei vorhandenen Benutzerkonten ab.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-107">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span>
4. <span data-ttu-id="6e6e6-108">Wechseln Sie zu Windows-Einstellungen > **Konten**  >  **e-Mail-& Konten**, und entfernen Sie alle Arbeits Konten mit Ausnahme des betroffenen Kontos.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-108">Go to Windows Settings > **Accounts** > **Email & accounts**, and remove all work accounts except the affected account.</span></span>
5. <span data-ttu-id="6e6e6-109">Wechseln Sie zu Windows-Einstellungen > **Konten**  >  **Zugriff auf Arbeit oder Schule**, und trennen Sie alle Arbeits Konten mit Ausnahme des betroffenen Kontos.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-109">Go to Windows Settings > **Accounts** > **Access work or school**, and disconnect all work accounts except the affected account.</span></span>
6. <span data-ttu-id="6e6e6-110">Setzen Sie den Office-Aktivierungsstatus zurück.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-110">Reset the Office activation state.</span></span> <span data-ttu-id="6e6e6-111">[Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="6e6e6-111">[Learn how](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span>
7. <span data-ttu-id="6e6e6-112">[Melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mit dem betroffenen Benutzerkonto an.</span><span class="sxs-lookup"><span data-stu-id="6e6e6-112">[Sign in](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>

<span data-ttu-id="6e6e6-113">Weitere Problem Behandlungslösungen finden Sie unter nicht [lizenziertes Produkt und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="6e6e6-113">For additional troubleshooting solutions, see [Unlicensed Product and activation errors in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>