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
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390422"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="0e525-102">Problembehandlung bei der Kennwortsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="0e525-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="0e525-103">Zur Behandlung von Problemen, bei denen keine Kennwörter mit Azure AD Connect-Version 1.1.614.0 oder höher synchronisiert werden:</span><span class="sxs-lookup"><span data-stu-id="0e525-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="0e525-104">Öffnen Sie auf Ihrem Azure AD Connect-Server eine neue Windows PowerShell-Sitzung mit der Option **als Administrator ausführen** .</span><span class="sxs-lookup"><span data-stu-id="0e525-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="0e525-105">Führen Sie **Set-ExecutionPolicy RemoteSigned** oder **Set-ExecutionPolicy Unrestricted**aus.</span><span class="sxs-lookup"><span data-stu-id="0e525-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="0e525-106">Starten Sie den Azure AD Connect-Assistenten.</span><span class="sxs-lookup"><span data-stu-id="0e525-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="0e525-107">Navigieren Sie zu der Seite \* \* zusätzliche Aufgaben \* \*, wählen Sie \* \* Problembehandlung \* \* aus, und klicken Sie auf **weiter**.</span><span class="sxs-lookup"><span data-stu-id="0e525-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="0e525-108">Klicken Sie auf der Seite Problembehandlung auf **Start, um das Menü Problembehandlung in PowerShell zu starten** .</span><span class="sxs-lookup"><span data-stu-id="0e525-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="0e525-109">Wählen Sie im Hauptmenü die Option **Problembehandlung für Kennwortsynchronisierung**aus.</span><span class="sxs-lookup"><span data-stu-id="0e525-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="0e525-110">Wählen Sie im Untermenü die Option **Kennwortsynchronisierung funktioniert nicht**aus.</span><span class="sxs-lookup"><span data-stu-id="0e525-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="0e525-111">**GrundLegendes zu den Ergebnissen der Problem Behandlungs Aufgabe**</span><span class="sxs-lookup"><span data-stu-id="0e525-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="0e525-112">Die Problem Behandlungs Aufgabe führt die folgenden Prüfungen aus:</span><span class="sxs-lookup"><span data-stu-id="0e525-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="0e525-113">Überprüft, ob die Kennwortsynchronisierung für Ihren Azure AD-Mandanten aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0e525-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="0e525-114">Überprüft, ob sich der Azure AD Connect-Server nicht im stagingmodus befindet.</span><span class="sxs-lookup"><span data-stu-id="0e525-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="0e525-115">Für jeden vorhandenen lokalen Active Directory-Connector (der einer vorhandenen Active Directory-Gesamtstruktur entspricht):</span><span class="sxs-lookup"><span data-stu-id="0e525-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="0e525-116">Überprüft, ob die Kennwortsynchronisierung aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="0e525-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="0e525-117">Sucht in den Ereignisprotokollen der Windows-Anwendung nach Kenn Wort Synchronisierungs Takt Ereignissen.</span><span class="sxs-lookup"><span data-stu-id="0e525-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="0e525-118">Für jede Active Directory-Domäne unter dem lokalen Active Directory-Connector:</span><span class="sxs-lookup"><span data-stu-id="0e525-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="0e525-119">Überprüft, ob die Domäne vom Azure AD Connect-Server erreichbar ist.</span><span class="sxs-lookup"><span data-stu-id="0e525-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="0e525-120">Überprüft, ob die vom lokalen Active Directory Connector verwendeten Active Directory-Domänendienste (AD DS)-Konten über den richtigen Benutzernamen, das richtige Kennwort und die für die Kennwortsynchronisierung erforderlichen Berechtigungen verfügen.</span><span class="sxs-lookup"><span data-stu-id="0e525-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="0e525-121">Weitere Hilfe bei der Problembehandlung bei der Kennwortsynchronisierung finden Sie unter [Problembehandlung bei der Kennwortsynchronisierung mit Azure AD Connect Sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="0e525-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

