---
title: Problembehandlung bei kennwortsynchronisierung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: c71fce8621057093d23891c26f7b0285fdc8b9ed
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/15/2019
ms.locfileid: "28289839"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="f7ec4-102">Problembehandlung bei kennwortsynchronisierung</span><span class="sxs-lookup"><span data-stu-id="f7ec4-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="f7ec4-103">Zum Behandeln von Problemen, wenn keine Kennwörter mit Azure AD-Connect Version 1.1.614.0 synchronisiert oder höher sind:</span><span class="sxs-lookup"><span data-stu-id="f7ec4-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="f7ec4-104">Öffnen Sie eine neue Windows PowerShell-Sitzung auf dem Server Azure AD-Verbinden mit der Option **als Administrator ausführen** .</span><span class="sxs-lookup"><span data-stu-id="f7ec4-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="f7ec4-105">Führen Sie **Set-ExecutionPolicy RemoteSigned** oder **Set-ExecutionPolicy Unrestricted**.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="f7ec4-106">Starten Sie den Assistenten Azure Active Directory verbinden.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="f7ec4-107">Navigieren Sie zu der \*\* zusätzliche Aufgaben \*\* Seite auf \*\* Troubleshoot \*\*, und klicken Sie auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="f7ec4-108">Klicken Sie auf der Seite Problembehandlung auf in PowerShell im Menü **Start um die Problembehandlung zu starten** .</span><span class="sxs-lookup"><span data-stu-id="f7ec4-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="f7ec4-109">Wählen Sie im Hauptmenü **Kennwortsynchronisierung behandeln**.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="f7ec4-110">Wählen Sie im Menü Sub **Kennwortsynchronisierung funktioniert nicht in allen**.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="f7ec4-111">**Verstehen der Ergebnisse des Vorgangs zur Problembehandlung**</span><span class="sxs-lookup"><span data-stu-id="f7ec4-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="f7ec4-112">Der Problembehandlung Task führt die folgenden überprüft:</span><span class="sxs-lookup"><span data-stu-id="f7ec4-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="f7ec4-113">Überprüft, dass das Synchronisierungsfeature Kennwort für Ihren Azure AD-Mandanten aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="f7ec4-114">Überprüft, dass der Azure AD-Connect-Server nicht ist in der staging-Modus.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="f7ec4-115">Für jeden vorhandenen lokalen Active Directory Connector (der vorhandenen Active Directory-Gesamtstruktur entspricht):</span><span class="sxs-lookup"><span data-stu-id="f7ec4-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="f7ec4-116">Überprüft, dass die Funktion "Kennwort Synchronisierung" aktiviert ist.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="f7ec4-117">Sucht nach Kennwort Synchronisierung Heartbeat-Ereignisse in der Windows-Anwendungsereignisprotokolle.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="f7ec4-118">Für jede Active Directory-Domäne unter der lokalen Active Directory-Verbindung:</span><span class="sxs-lookup"><span data-stu-id="f7ec4-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="f7ec4-119">Überprüft, ob die Domäne aus dem Azure AD-Connect Server erreichbar ist.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="f7ec4-120">Überprüft, dass die Active Directory-Domänendienste (AD DS)-Konten, die von der lokalen Active Directory-Verbindung verwendet wurde, die richtige Benutzername, Kennwort und erforderliche Berechtigungen für die Synchronisierung von Kennwörtern.</span><span class="sxs-lookup"><span data-stu-id="f7ec4-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="f7ec4-121">Weitere Hilfe zur Problembehandlung für Kennwort Sync finden Sie unter [Troubleshoot kennwortsynchronisierung mit Azure AD-Connect-Synchronisierung](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="f7ec4-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

