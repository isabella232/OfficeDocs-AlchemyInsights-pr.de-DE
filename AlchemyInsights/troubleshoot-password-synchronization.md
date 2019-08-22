---
title: Problembehandlung bei der Kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 2b0a1527ab1b16f56a97891445a2dcb4570302f5
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533806"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="92162-102">Problembehandlung bei der Kennwortsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="92162-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="92162-103">Zur Behandlung von Problemen, bei denen keine Kennwörter mit Azure AD Connect-Version 1.1.614.0 oder höher synchronisiert werden:</span><span class="sxs-lookup"><span data-stu-id="92162-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="92162-104">Öffnen Sie eine neue Windows PowerShell Sitzung auf Ihrem Azure AD Connect-Server mit der Option **als Administrator ausführen** .</span><span class="sxs-lookup"><span data-stu-id="92162-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="92162-105">Führen Sie " **ExecutionPolicy RemoteSigned** " oder " **festgelegt-ExecutionPolicy Unrestricted**" aus.</span><span class="sxs-lookup"><span data-stu-id="92162-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="92162-106">Starten Sie den Azure AD Connect-Assistenten.</span><span class="sxs-lookup"><span data-stu-id="92162-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="92162-107">Navigieren Sie zur Seite **Weitere Aufgaben** , wählen Sie **Problembehandlung**aus, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="92162-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="92162-108">Klicken Sie auf der Seite Problembehandlung auf **starten, um das Menü Problembehandlung in PowerShell zu starten** .</span><span class="sxs-lookup"><span data-stu-id="92162-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="92162-109">Wählen Sie im Hauptmenü die Option **Problembehandlung für die Kennwortsynchronisierung**aus.</span><span class="sxs-lookup"><span data-stu-id="92162-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="92162-110">Wählen Sie im Untermenü die Option **Kennwortsynchronisierung funktioniert überhaupt nicht**aus.</span><span class="sxs-lookup"><span data-stu-id="92162-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="92162-111">**Grundlegendes zu den Ergebnissen der Aufgaben zur Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="92162-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="92162-112">Die Problem Behandlungs Aufgabe führt die folgenden Prüfungen durch:</span><span class="sxs-lookup"><span data-stu-id="92162-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="92162-113">Überprüft, ob das Feature für die Kennwortsynchronisierung für den Azure AD Mandanten aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="92162-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="92162-114">Überprüft, ob sich der Azure AD Connect-Server nicht im stagingmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="92162-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="92162-115">Für jeden vorhandenen lokalen Active Directory Connector (der einer vorhandenen Active Directory Gesamtstruktur entspricht):</span><span class="sxs-lookup"><span data-stu-id="92162-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="92162-116">Überprüft, ob das Feature für die Kennwortsynchronisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="92162-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="92162-117">Sucht nach Kenn Wort Synchronisierungs Takt Ereignissen in den Windows-Anwendungsereignisprotokollen.</span><span class="sxs-lookup"><span data-stu-id="92162-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="92162-118">Für jede Active Directory Domäne unter dem lokalen Active Directory Connector:</span><span class="sxs-lookup"><span data-stu-id="92162-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="92162-119">Überprüft, ob die Domäne über den Azure AD Connect-Server erreichbar ist.</span><span class="sxs-lookup"><span data-stu-id="92162-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="92162-120">Überprüft, ob die vom lokalen Active Directory Connector verwendeten Active Directory-Domänendienste Konten (AD DS) über den korrekten Benutzernamen, das Kennwort und die erforderlichen Berechtigungen für die Kennwortsynchronisierung verfügen.</span><span class="sxs-lookup"><span data-stu-id="92162-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="92162-121">Weitere Hilfe zur Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="92162-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  