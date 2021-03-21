---
title: Konfigurieren Sie den Dienstverbindungspunkts (SCP).
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50898064"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="6b428-102">Konfigurieren Sie den Dienstverbindungspunkt (SCP).</span><span class="sxs-lookup"><span data-stu-id="6b428-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="6b428-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="6b428-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="6b428-104">**Grund**: Das SCP-Objekt kann nicht gelesen und die Azure AD-Mandanteninformationen können nicht abgerufen werden</span><span class="sxs-lookup"><span data-stu-id="6b428-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="6b428-105">**Lösung**: Weitere Informationen finden Sie im Abschnitt [Konfigurieren eines Dienstverbindungspunkts](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span><span class="sxs-lookup"><span data-stu-id="6b428-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="6b428-106">**Aktionsplan**</span><span class="sxs-lookup"><span data-stu-id="6b428-106">**Action plan**</span></span>

- <span data-ttu-id="6b428-107">Überprüfen Sie, ob das Gerät das Gruppenrichtlinienobjekt für die kontrollierte Prüfung erhalten hat.</span><span class="sxs-lookup"><span data-stu-id="6b428-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="6b428-108">Stellen Sie sicher, dass das Gruppenrichtlinienobjekt die Registrierungsschlüssel erstellt hat.</span><span class="sxs-lookup"><span data-stu-id="6b428-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="6b428-109">Stellen Sie sicher, dass Sie 2 Schlüssel mit Ihrer Verzeichnis-ID und Ihrer Onmicrosoft-Domäne erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="6b428-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="6b428-110">**Konfigurieren der clientseitigen Registrierungseinstellung für SCP**</span><span class="sxs-lookup"><span data-stu-id="6b428-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="6b428-111">Verwenden Sie das folgende Beispiel, um ein Gruppenrichtlinienobjekt (Group Policy Object, GPO) zu erstellen, um eine Registrierungseinstellung bereitzustellen, mit der ein SCP-Eintrag in der Registrierung Ihrer Geräte konfiguriert wird.</span><span class="sxs-lookup"><span data-stu-id="6b428-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="6b428-112">Öffnen Sie eine Gruppenrichtlinien-Verwaltungskonsole und erstellen Sie ein neues Gruppenrichtlinienobjekt in Ihrer Domäne.</span><span class="sxs-lookup"><span data-stu-id="6b428-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="6b428-113">Geben Sie Ihrem neu erstellten Gruppenrichtlinienobjekt einen Namen (z. B. ClientSideSCP).</span><span class="sxs-lookup"><span data-stu-id="6b428-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="6b428-114">Bearbeiten Sie das Gruppenrichtlinienobjekt und suchen Sie den folgenden Pfad: **Computerkonfiguration > Einstellungen > Windows-Einstellungen > Registrierung**.</span><span class="sxs-lookup"><span data-stu-id="6b428-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="6b428-115">Klicken Sie mit der rechten Maustaste auf **Registrierung** und wählen Sie **Neu > Registrierungselement**.</span><span class="sxs-lookup"><span data-stu-id="6b428-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="6b428-116">Auf der Registerkarte **Allgemein** konfigurieren Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="6b428-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6b428-117">**Aktion**: Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6b428-117">**Action**: Update</span></span>
    
- <span data-ttu-id="6b428-118">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6b428-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6b428-119">**Schlüsselpfad**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6b428-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6b428-120">**Wertname**: TenantId</span><span class="sxs-lookup"><span data-stu-id="6b428-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="6b428-121">**Werttyp**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6b428-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6b428-122">**Wertdaten**: Die GUID oder Verzeichnis-ID Ihrer Azure AD-Instanz (Dieser Wert befindet sich unter **Azure-Portal > Azure Active Directory > Eigenschaften > Verzeichnis-ID**)</span><span class="sxs-lookup"><span data-stu-id="6b428-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="6b428-123">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="6b428-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="6b428-124">Klicken Sie mit der rechten Maustaste auf **Registrierung** und wählen Sie **Neu > Registrierungselement**.</span><span class="sxs-lookup"><span data-stu-id="6b428-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="6b428-125">Auf der Registerkarte **Allgemein** konfigurieren Sie Folgendes:</span><span class="sxs-lookup"><span data-stu-id="6b428-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="6b428-126">**Aktion**: Aktualisieren</span><span class="sxs-lookup"><span data-stu-id="6b428-126">**Action**: Update</span></span>
    
- <span data-ttu-id="6b428-127">**Hive**: HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="6b428-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="6b428-128">**Schlüsselpfad**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="6b428-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="6b428-129">**Wertname**: TenantName</span><span class="sxs-lookup"><span data-stu-id="6b428-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="6b428-130">**Werttyp**: REG_SZ</span><span class="sxs-lookup"><span data-stu-id="6b428-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="6b428-131">**Wertdaten**: Ihr verifizierter Domänenname, wenn Sie eine Verbundumgebung wie AD FS verwenden.</span><span class="sxs-lookup"><span data-stu-id="6b428-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="6b428-132">Ihr verifizierter Domainname oder Ihr Domainname onmicrosoft.com (z. B. contoso.onmicrosoft).com, wenn Sie eine verwaltete Umgebung verwenden</span><span class="sxs-lookup"><span data-stu-id="6b428-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="6b428-133">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="6b428-133">Click **OK**.</span></span>

7. <span data-ttu-id="6b428-134">Schließen Sie den Editor für das neu erstellte Gruppenrichtlinienobjekt.</span><span class="sxs-lookup"><span data-stu-id="6b428-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="6b428-135">Verknüpfen Sie das neu erstellte Gruppenrichtlinienobjekt mit der gewünschten Organisationseinheit, die domänenverbundene Computer enthält, die zu Ihrer kontrollierten Rollout-Population gehören.</span><span class="sxs-lookup"><span data-stu-id="6b428-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="6b428-136">Weitere Informationen finden Sie unter [Kontrollierte Prüfung des hybriden Azure AD-Joins – Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) und  [Fehlerbehebung für hybride Azure Active Directory-Geräte | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span><span class="sxs-lookup"><span data-stu-id="6b428-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









