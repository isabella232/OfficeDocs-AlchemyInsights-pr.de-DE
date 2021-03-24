---
title: Suchen fehlender Anwendungen auf dem Blatt App-Registrierung
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
- "9004352"
- "9654"
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/23/2021
ms.locfileid: "51123091"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Suchen fehlender Anwendungen auf dem Blatt App-Registrierung

1. Anwendungen im App-Registrierungsportal können nicht angezeigt werden.

    Wenn es sich bei einer Anwendung um eine mehrstufige Anwendung handelt und sie in einem anderen Mandanten registriert wurde, wird sie nicht unter dem Blatt App-Registrierung angezeigt. Möglicherweise finden Sie sie jedoch unter Dem Blatt Enterprise-Anwendungen, nachdem auf sie zugegriffen wurde (nachdem sie zugestimmt wurde) und der Dienstprinzipal in Ihrem Mandanten erstellt wurde. Weitere Informationen finden Sie unter [Apps & service principals in Azure AD - Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Apps können nicht im Blatt App-Registrierung angezeigt werden, obwohl Sie Administrator sind.

    Stellen Sie sicher, dass Sie sich im richtigen Verzeichnis im Azure-Portal befinden.
3. Meine Anwendung ist nicht unter Dem Blatt Enterprise-Anwendungen aufgeführt, wird aber angezeigt, wenn ich den PowerShell-Befehl abfordere.

    Manchmal wird die Anwendung nach dem Löschen aus dem Azure-Portal nicht im Portal angezeigt, aber möglicherweise nicht vollständig gelöscht. Weitere Informationen finden Sie unter:
    - Sie können die Liste der zuvor gelöschten Anwendungen abrufen und mit dem Befehl Powershell sehen, ob die Anwendung in der Liste angezeigt **wird: Get-AzureADDeletedApplication**. Weitere Informationen finden Sie unter [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Wenn Sie die Anwendung vollständig entfernen möchten, können Sie Folgendes in PowerShell ausprobieren: **Remove-AzureADApplication -ObjectId**. Weitere Informationen finden Sie unter [Remove-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Alternativ können Sie versuchen, die gelöschte Anwendung mithilfe des folgenden Powershell-Befehls wiederherzustellen: **AzureADDeletedApplication -ObjectId wiederherstellen.** Weitere Informationen finden Sie unter [Restore-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Liste aller vorinstallierten Unternehmensanwendungen in meinem neuen Azure-Mandanten nicht finden.

    Es gibt standardmäßig keine vorinstallierten Unternehmensanwendungen in Azure AD. Sie müssen sie manuell über die Option Neue Anwendung hinzufügen, indem Sie sie aus dem Azure AD-Katalog durchsuchen oder eine Nicht-Katalog-Anwendung hinzufügen. Weitere Informationen finden Sie unter Schnellstart: Hinzufügen einer Anwendung zu Ihrem [Azure Active Directory (Azure AD)-Mandanten.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Wenn Sie ein globaler Administrator sind, können Sie ganz einfach über die [Microsoft 365-App-Startprogramm.](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher)
5. Meine Apps können im Portal "Meine Apps" nicht angezeigt werden.

    Stellen Sie sicher, dass Apps nicht auf der Sammlungsseite "Meine Apps" ausgeblendet sind. Weitere Informationen finden Sie unter [Sammlungen (Vorschau) im Portal "Meine Apps" – Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Informationen zum Starten von Apps aus dem Portal "Meine Apps" finden Sie unter [Locate & use apps on the My Apps portal - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Die Office 365 Mover-App wird nach der Installation nicht auf dem Blatt Enterprise Applications angezeigt.

    Die "Office 365 Mover"-Anwendung ist eine mehrstufige App, die AAD nicht mithilfe des Abschnitts Galerieanwendungen unter Enterprise App Registration hinzugefügt werden muss. Um auf die Office 365 Mover-App zu zugreifen, melden Sie sich einfach bei der App an, und sie würde die Zustimmung des Benutzers für die Berechtigungen einholen. Sobald der Benutzer die Zustimmung erteilt hat, wird diese App automatisch dem Mandanten mit der E-Mail-ID hinzugefügt, die Sie angemeldet haben.

    Nach der Anmeldung bei der Anwendung sollten Sie in der Lage sein, den Eintrag dieser Anwendung unter dem Blatt Enterprise Applications in AAD zu finden. Sie müssen nach dieser Anwendung suchen, indem Sie entweder den vollständigen Namen eingeben, d. h. "Office 365 Mover" oder einfach "Office" suchen und die App auflisten. Weitere Informationen finden Sie unter [Office 365 Mover,](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html)dass es bereits installiert ist, aber nicht im Katalog enterprise application aufgeführt ist.
8. Schnellstart: In der Liste der Anwendungen, die Ihren [Azure Active Directory (Azure AD)-Mandanten](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) für die Identitätsverwaltung verwenden, erfahren Sie, wie Sie die Anwendungen anzeigen, die bereits für die Verwendung Ihres Azure AD-Mandanten als Identitätsanbieter (IdP) eingerichtet sind.
9. [Die Problembehandlung bei häufigen Problemen](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) beim Hinzufügen oder Entfernen einer Anwendung zu Azure Active Directory hilft Ihnen, die häufigen Probleme zu verstehen, mit denen Benutzer Apps in Azure Active Directory anzeigen müssen.
