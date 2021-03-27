---
title: Eine Liste der Unternehmensanwendungen erhalten
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/26/2021
ms.locfileid: "51379851"
---
# <a name="get-a-list-of-enterprise-applications"></a>Eine Liste der Unternehmensanwendungen erhalten

1. Eine Liste **der** Unternehmensanwendungen (alle Anwendungen oder gefiltert nach Anzeigename, ID, BEZEICHNER-URIs usw.) über den Befehl Powershell finden Sie unter [Get-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Eine Liste der Dienstprinzipalobjekte (alle Objekte oder gefiltert nach ID) über den Befehl Powershell finden Sie unter [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Wenn Sie eine Liste der samlkonfigurierten Apps erhalten möchten, können Ihnen die folgenden **PowerShell-Skripts** helfen:

    Jede Anwendung, sei es eine OAuth-App oder eine SAML-App (sowohl Katalog- als auch Nicht-Katalog-Apps), würde zwei Objekte in AAD erstellen, wenn ihre Registrierung erfolgt. Eines wird als Application-Objekt bezeichnet, das andere als Dienstprinzipalobjekt. Wenn Sie die Eigenschaften eines Dienstprinzipalobjekts mithilfe von PowerShell abbilden, stellen Sie fest, dass jeder Anwendung eine bestimmte Anzahl von Tags zugeordnet ist, wie:

    - OAuth-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps hätte ein Tag namens "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Nicht-Gallery-SAML-Apps hätten ein Tag namens "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Daher können Sie diese Tags verwenden und herausfinden, um welche Art von App es sich handelt. Das Tag "**WindowsAzureActiveDirectoryIntegratedApp**" ist für alle Arten von Apps üblich. Sie können den folgenden Codeausschnitt verwenden, um alle SAML-Apps (sowohl Katalog als auch Nicht-Katalog) auflisten:

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Weitere Informationen finden Sie unter [Identifizieren von SAML-aktivierten Apps in Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Nur Webanwendungen** suchen und auflisten: Verwenden Sie den folgenden Befehl, um alle Azure AD-Anwendungen mit dem Anwendungstyp "Web-App/API" zu erhalten.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Nur systemeigene Anwendungen suchen und auflisten:** Führen Sie den folgenden Befehl aus, um alle systemeigenen Clientanwendungen (Desktop-/Mobilgeräte) zu erhalten.

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. **Export All Registered Azure AD Application Details to CSV**: Der folgende Befehl exportiert alle Azure AD-Apps mit den erforderlichen Details in eine CSV-Datei:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Müssen eine Liste nicht verwendeter Azure-Apps exportieren** – Überwachungsbericht

    Azure AD kann Anwendungsprotokolle nur für bis zu 30 Tage anzeigen, vorausgesetzt, Sie haben Azure AD Premium-Lizenz.
    Sie haben zwei Optionen, um die Daten länger als 30 Tage zu speichern. Sie können die [Azure AD Reporting-APIs](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) verwenden, um die Daten programmgesteuert abzurufen und in einer Datenbank zu speichern. Alternativ können Sie Überwachungsprotokolle in ein SIEM-System eines Drittanbieters integrieren.

    Sie können auch die App-Liste für alle Anwendungen und im Besitz von Anwendungen unter Azure Active Directory>App Registrations>Download>All applications/Owned applications herunterladen.

    Eine Liste der Anwendungen über MS Graph finden Sie unter [List applications - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) and application resource type - Microsoft Graph [v1.0](https://docs.microsoft.com/graph/api/resources/application).
