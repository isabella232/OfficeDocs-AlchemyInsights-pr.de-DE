---
title: Kennwortprotokolle
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523085"
---
# <a name="password-logs"></a><span data-ttu-id="b54f8-102">Kennwortprotokolle</span><span class="sxs-lookup"><span data-stu-id="b54f8-102">Password logs</span></span>

<span data-ttu-id="b54f8-103">**Ich habe Probleme beim Zugriff auf Überwachungsprotokolle für die Kennwortzurücksetzung**</span><span class="sxs-lookup"><span data-stu-id="b54f8-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="b54f8-104">Führen Sie den folgenden Schritt aus, um Probleme im Zusammenhang mit dem Zugriff auf Überwachungsprotokolle für die Kennwortzurücksetzung zu behandeln:</span><span class="sxs-lookup"><span data-stu-id="b54f8-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="b54f8-105">Stellen Sie sicher, dass Sie zum Anzeigen von Überwachungsprotokollen autorisiert sind.</span><span class="sxs-lookup"><span data-stu-id="b54f8-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="b54f8-106">Nur die folgenden Rollen sind autorisiert:</span><span class="sxs-lookup"><span data-stu-id="b54f8-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="b54f8-107">Globaler Administrator</span><span class="sxs-lookup"><span data-stu-id="b54f8-107">Global administrator</span></span>
 - <span data-ttu-id="b54f8-108">Sicherheitsadministrator</span><span class="sxs-lookup"><span data-stu-id="b54f8-108">Security administrator</span></span>
 - <span data-ttu-id="b54f8-109">Benutzer mit Leseberechtigung für Sicherheitsfunktionen</span><span class="sxs-lookup"><span data-stu-id="b54f8-109">Security reader</span></span>

<span data-ttu-id="b54f8-110">**Ich möchte alle Überwachungsereignisse für die Kennwortzurücksetzung ab der ersten Bereitstellung sehen**</span><span class="sxs-lookup"><span data-stu-id="b54f8-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="b54f8-111">In den Berichten der letzten 30 Tage wurden bis zu 120.000 Kennwortzurücksetzungs-/Registrierungsereignisse gespeichert.</span><span class="sxs-lookup"><span data-stu-id="b54f8-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="b54f8-112">Dieses maximale Limit gilt für die Benutzeroberfläche beim Herunterladen der CSV-Datei.</span><span class="sxs-lookup"><span data-stu-id="b54f8-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="b54f8-113">1 Million Ereignisse stehen über PowerShell zur Verfügung.</span><span class="sxs-lookup"><span data-stu-id="b54f8-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="b54f8-114">Weitere Informationen finden Sie in den nachfolgenden Tipps:</span><span class="sxs-lookup"><span data-stu-id="b54f8-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="b54f8-115">Self-Service-Kennwortzurücksetzungsereignisse aus den Azure AD-Berichts- und -Ereignis-API</span><span class="sxs-lookup"><span data-stu-id="b54f8-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="b54f8-116">Schnelles Herunterladen von Registrierungsereignissen für die Kennwortzurücksetzung mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="b54f8-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="b54f8-117">**Ich möchte mehr über die Berichterstellungsfunktionen für die Kennwortzurücksetzung erfahren**</span><span class="sxs-lookup"><span data-stu-id="b54f8-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="b54f8-118">Überprüfen Sie im Azure-Portal unter **„Benutzer und Gruppen"**, wer Kennwörter mit Azure AD-Protokollen zur Kennwortzurücksetzung registriert oder zurücksetzt.</span><span class="sxs-lookup"><span data-stu-id="b54f8-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="b54f8-119">Weitere Informationen finden Sie unter den folgenden Links:</span><span class="sxs-lookup"><span data-stu-id="b54f8-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="b54f8-120">Übersicht über das Zurücksetzen von Kennwörtern</span><span class="sxs-lookup"><span data-stu-id="b54f8-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="b54f8-121">Anzeigen von Berichten zur Kennwortzurücksetzung im Azure-Portal</span><span class="sxs-lookup"><span data-stu-id="b54f8-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="b54f8-122">Self-Service-Kennwortzurücksetzungsereignisse aus den Azure AD-Berichts- und -Ereignis-API</span><span class="sxs-lookup"><span data-stu-id="b54f8-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="b54f8-123">Schnelles Herunterladen von Registrierungsereignissen für die Kennwortzurücksetzung mit PowerShell</span><span class="sxs-lookup"><span data-stu-id="b54f8-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


