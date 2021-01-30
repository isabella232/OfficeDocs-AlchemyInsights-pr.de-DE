---
title: Probleme mit Anmeldeinformationen
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004330"
- "7723"
ms.openlocfilehash: e463e8181123277f3509c0b0bb6f871a1a09bed1
ms.sourcegitcommit: c3574f574afe5a40a6ea2c6e399c58977d18bb73
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/29/2021
ms.locfileid: "50052948"
---
# <a name="issues-with-credentials"></a><span data-ttu-id="ca484-102">Probleme mit Anmeldeinformationen</span><span class="sxs-lookup"><span data-stu-id="ca484-102">Issues with credentials</span></span>

<span data-ttu-id="ca484-103">Microsoft Identity Platform und der [OAuth 2.0-Clientanmeldeinformationsfluss](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) beschreiben, wie Sie direkt mit dem OAuth 2.0-Client-Anmeldeinformations-Genehmigungsfluss programmieren.</span><span class="sxs-lookup"><span data-stu-id="ca484-103">[Microsoft identity platform and the OAuth 2.0 client credentials flow](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) describes how to program directly against the OAuth 2.0 client credentials grant flow.</span></span>

<span data-ttu-id="ca484-104">**Wie verwalte ich das Kennwort oder die Zertifikatanmeldeinformationen einer Anwendung?**</span><span class="sxs-lookup"><span data-stu-id="ca484-104">**How do I manage an application's password or certificate credentials?**</span></span>

<span data-ttu-id="ca484-105">In der Azure CLI können Sie az [ad-App-Anmeldeinformationen](https://docs.microsoft.com/cli/azure/ad/app/credential) verwenden, um das Kennwort oder das Zertifikat einer Anwendung zu löschen, auflisten oder zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-105">In the Azure CLI, you can use [az ad app credential](https://docs.microsoft.com/cli/azure/ad/app/credential) to delete, list, or reset an application's password or certificate credentials.</span></span>

<span data-ttu-id="ca484-106">**Wie setzen meine Benutzer ihre Kennwörter zurück?**</span><span class="sxs-lookup"><span data-stu-id="ca484-106">**How do my users reset their passwords?**</span></span>

<span data-ttu-id="ca484-107">Benutzer müssen sich [für die Self-Service-Kennwortzurücksetzung registrieren,](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) bevor sie ihre Kennwörter zurücksetzen können.</span><span class="sxs-lookup"><span data-stu-id="ca484-107">Users need to [register for self-service password reset](https://docs.microsoft.com/azure/active-directory/user-help/active-directory-passwords-reset-register) before they can reset their passwords.</span></span> <span data-ttu-id="ca484-108">Nachdem sich ein Benutzer registriert hat, kann er den Anweisungen in diesem Artikel folgen, um sein Kennwort zurückzusetzen: [Zurücksetzen des Arbeits-](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account)oder Schulkennworts.</span><span class="sxs-lookup"><span data-stu-id="ca484-108">Once a user has registered, they can follow the instructions in this article to reset their password: [Reset your work or school password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-reset-or-unlock-your-password-for-a-work-or-school-account).</span></span>

<span data-ttu-id="ca484-109">**Wie ändern meine Benutzer ihre Kennwörter?**</span><span class="sxs-lookup"><span data-stu-id="ca484-109">**How do my users change their passwords?**</span></span>

<span data-ttu-id="ca484-110">Benutzer können die Schritte in diesem Artikel ausführen, um ihre Kennwörter zu ändern: [So ändern Sie Ihr Kennwort.](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password)</span><span class="sxs-lookup"><span data-stu-id="ca484-110">Users can follow the steps in this article to change their passwords: [How to change your password](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#how-to-change-your-password).</span></span>
<span data-ttu-id="ca484-111">Sie können auch [App-Kennwörter für die Überprüfung in zwei Schritten verwalten.](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords)</span><span class="sxs-lookup"><span data-stu-id="ca484-111">They can also [Manage app passwords for two-step verification](https://docs.microsoft.com/azure/active-directory/user-help/multi-factor-authentication-end-user-app-passwords).</span></span>

<span data-ttu-id="ca484-112">**Mein Benutzer wird beim Ändern oder Zurücksetzen des Kennworts einen Fehler erhalten.**</span><span class="sxs-lookup"><span data-stu-id="ca484-112">**My user is getting an error when changing or resetting their password**</span></span>

<span data-ttu-id="ca484-113">Dieser Link enthält Informationen zu häufigen Problemen, die auftreten können, wenn ein Benutzer versucht, sein Kennwort zurückzusetzen: Häufige [Probleme und deren Lösungen](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span><span class="sxs-lookup"><span data-stu-id="ca484-113">This link will provide information on common problems that can arise when a user is trying to reset their password: [Common problems and their solutions](https://docs.microsoft.com/azure/active-directory/user-help/user-help-reset-password#common-problems-and-their-solutions)</span></span>

<span data-ttu-id="ca484-114">**Ich habe ein Problem beim Zurücksetzen des Kennworts eines Benutzers**</span><span class="sxs-lookup"><span data-stu-id="ca484-114">**I'm having a problem resetting a user's password**</span></span>

- <span data-ttu-id="ca484-115">Stellen Sie sicher, dass Sie zum Zurücksetzen von Kennwörtern autorisiert sind.</span><span class="sxs-lookup"><span data-stu-id="ca484-115">Make sure you are authorized to reset passwords.</span></span> <span data-ttu-id="ca484-116">*Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.*</span><span class="sxs-lookup"><span data-stu-id="ca484-116">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ca484-117">Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-117">Global administrators can also reset other privileged administrator's passwords.</span></span>

- <span data-ttu-id="ca484-118">Stellen Sie sicher, dass Sie die Lizenzierungsanforderungen verstehen:</span><span class="sxs-lookup"><span data-stu-id="ca484-118">Make sure you understand the licensing requirements:</span></span>

  - <span data-ttu-id="ca484-119">Ihnen muss mindestens eine Lizenz in Ihrer Organisation zugewiesen sein:</span><span class="sxs-lookup"><span data-stu-id="ca484-119">You must have at least one license assigned in your organization:</span></span>
    - <span data-ttu-id="ca484-120">**Nur Cloudbenutzer** – jede kostenpflichtige Office 365 (O365)-SKU oder Azure AD Basic</span><span class="sxs-lookup"><span data-stu-id="ca484-120">**Cloud only users** - Any Office 365 (O365) paid SKU, or Azure AD Basic</span></span>
    - <span data-ttu-id="ca484-121">**Cloud- und/oder lokale** Benutzer – Azure AD Premium P1 oder P2, Enterprise Mobility + Security (EMS) oder Secure Productive Enterprise (SPE)</span><span class="sxs-lookup"><span data-stu-id="ca484-121">**Cloud and/or on-premises users** - Azure AD Premium P1 or P2, Enterprise Mobility + Security (EMS), or Secure Productive Enterprise (SPE)</span></span>
    - <span data-ttu-id="ca484-122">Weitere Informationen zu Den Lizenzierungsanforderungen finden Sie unter Lizenzierungsanforderungen für die [Self-Service-Kennwortzurücksetzung in Azure AD.](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)</span><span class="sxs-lookup"><span data-stu-id="ca484-122">To learn more about licensing requirements, see [Licensing requirements for Azure AD self-service password reset](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing).</span></span>
- <span data-ttu-id="ca484-123">Um das Kennwort eines Benutzers zurückzusetzen, suchen Sie den Benutzer in Azure AD.</span><span class="sxs-lookup"><span data-stu-id="ca484-123">To reset a user's password, find the user in Azure AD.</span></span> <span data-ttu-id="ca484-124">Klicken Sie dann auf dem Blatt "Übersicht" für diesen Benutzer auf die Schaltfläche "Kennwort zurücksetzen".</span><span class="sxs-lookup"><span data-stu-id="ca484-124">Then, on the overview blade for that user, click the "reset password" button.</span></span>

<span data-ttu-id="ca484-125">**Die Schaltfläche zum Zurücksetzen des Kennworts ist ausgegraut.**</span><span class="sxs-lookup"><span data-stu-id="ca484-125">**The password reset button is greyed-out**</span></span>

<span data-ttu-id="ca484-126">Sie sind nicht autorisiert, die **Kennwörter dieses** Benutzers zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-126">You are not authorized to reset **this** user's passwords.</span></span> <span data-ttu-id="ca484-127">*Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.*</span><span class="sxs-lookup"><span data-stu-id="ca484-127">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ca484-128">Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-128">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ca484-129">**Ich kann das Blatt zum Zurücksetzen des Kennworts nicht sehen.**</span><span class="sxs-lookup"><span data-stu-id="ca484-129">**I don't see the password reset blade**</span></span>

<span data-ttu-id="ca484-130">Sie sind nicht autorisiert, Kennwörter zurückzusetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-130">You are not authorized to reset passwords.</span></span> <span data-ttu-id="ca484-131">*Nur globale, Kennwort- und Benutzeradministratoren können Benutzerkennwörter zurücksetzen.*</span><span class="sxs-lookup"><span data-stu-id="ca484-131">*Only global, password, and user administrators can reset user passwords.*</span></span> <span data-ttu-id="ca484-132">Globale Administratoren können auch die Kennwörter anderer privilegierter Administratoren zurücksetzen.</span><span class="sxs-lookup"><span data-stu-id="ca484-132">Global administrators can also reset other privileged administrator's passwords.</span></span>

<span data-ttu-id="ca484-133">**Ich kann das blatt für die lokale Integration bei der Kennwortzurücksetzung nicht sehen.**</span><span class="sxs-lookup"><span data-stu-id="ca484-133">**I don't see the on-premises integration blade in password reset**</span></span>

- <span data-ttu-id="ca484-134">Das blatt für die lokale Integration wird nur in Hybridumgebungen angezeigt, d. h., Sie verwenden das Kennwortrückschreiben, um die Kennwörter der lokalen Benutzer zu bearbeiten.</span><span class="sxs-lookup"><span data-stu-id="ca484-134">The on-premises integration blade only appears in hybrid environments - meaning you are using password writeback to manipulate on-premises user's passwords.</span></span>

- <span data-ttu-id="ca484-135">Dieses Blatt wird nicht angezeigt, wenn:</span><span class="sxs-lookup"><span data-stu-id="ca484-135">You do not see this blade if:</span></span>

  - <span data-ttu-id="ca484-136">Sie verwenden kein Kennwortrückschreiben</span><span class="sxs-lookup"><span data-stu-id="ca484-136">You are not using password writeback</span></span>
  - <span data-ttu-id="ca484-137">Es liegt ein Problem mit der Installation/Konnektivität des Kennwortrückschreibens vor.</span><span class="sxs-lookup"><span data-stu-id="ca484-137">There is a problem with your installation/connectivity of password writeback</span></span>
  - <span data-ttu-id="ca484-138">Es liegt ein Problem mit der Installation/Konnektivität von Azure AD Connect vor.</span><span class="sxs-lookup"><span data-stu-id="ca484-138">There is a problem with your installation/connectivity of Azure AD Connect</span></span>
  - <span data-ttu-id="ca484-139">Weitere Schritte zur Problembehandlung bei Problemen mit dem Kennwortrückschreiben finden Sie unter Problembehandlung beim [Kennwortrückschreiben.](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span><span class="sxs-lookup"><span data-stu-id="ca484-139">For more troubleshooting steps for issues with password writeback, see [Troubleshoot password writeback](https://docs.microsoft.com/azure/active-directory/authentication/troubleshoot-sspr-writeback)</span></span>

<span data-ttu-id="ca484-140">**Ich weiß nicht, wie ich das Kennwort eines Benutzers zurücksetzen kann.**</span><span class="sxs-lookup"><span data-stu-id="ca484-140">**I don't know how to reset a user's password**</span></span>

1. <span data-ttu-id="ca484-141">Melden Sie sich als entsprechender Administrator beim Azure-Portal an.</span><span class="sxs-lookup"><span data-stu-id="ca484-141">Sign in to the Azure portal as an appropriate admin.</span></span>
2. <span data-ttu-id="ca484-142">Wechseln Sie zum Blatt **"Benutzer und Gruppen",** und wählen **Sie "Alle Benutzer" aus.**</span><span class="sxs-lookup"><span data-stu-id="ca484-142">Go to the **Users and groups** blade, select **All Users**.</span></span>
3. <span data-ttu-id="ca484-143">Wählen Sie einen Benutzer aus der Liste aus.</span><span class="sxs-lookup"><span data-stu-id="ca484-143">Select a user from the list.</span></span>
4. <span data-ttu-id="ca484-144">Wählen Sie für den ausgewählten Benutzer **"Übersicht"** und dann in der Befehlsleiste **"Kennwort zurücksetzen" aus.**</span><span class="sxs-lookup"><span data-stu-id="ca484-144">For the selected user, select **Overview**, and then in the command bar, select **Reset password**.</span></span>
5. <span data-ttu-id="ca484-145">Wählen Sie die **Schaltfläche "Kennwort zurücksetzen"** aus, und folgen Sie den Anweisungen auf dem Bildschirm.</span><span class="sxs-lookup"><span data-stu-id="ca484-145">Select the **Reset password** button and follow the instructions on the screen.</span></span>
    - <span data-ttu-id="ca484-146">Nur Über das Azure-Portal durchgeführte **Zurücksetzungen unterstützen** das Kennwortrückschreiben.</span><span class="sxs-lookup"><span data-stu-id="ca484-146">Only resets performed through the **Azure portal** support password writeback.</span></span>

<span data-ttu-id="ca484-147">**Ich reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span><span class="sxs-lookup"><span data-stu-id="ca484-147">**I reset an on-premises user's password from the Office 365 Admin portal or Office 365 mobile application but the user is still not able to sign in**</span></span>

<span data-ttu-id="ca484-148">Das Rückschreiben von Kennwörtern wird in diesem Portal nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="ca484-148">Password Writeback is not supported in this portal.</span></span> <span data-ttu-id="ca484-149">Setzen Sie das Kennwort des Benutzers im Azure-Portal erneut zurück.</span><span class="sxs-lookup"><span data-stu-id="ca484-149">Reset the user's password again in the Azure portal.</span></span>
