---
title: Anmeldung bei Windows 10 ohne Verwendung eines Kennworts
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1f325eb7afb1e88457296e8187f8ba6dff2ebfe0
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588280"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="8108c-102">Anmeldung bei Windows 10 ohne Verwendung eines Kennworts</span><span class="sxs-lookup"><span data-stu-id="8108c-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="8108c-103">Um zu vermeiden, dass beim Windows-Start ein Kennwort eingegeben werden muss, empfehlen wir Ihnen, wenn verfügbar, eine der Windows Hello Secure-Anmeldeoptionen wie PIN, Face Recognition oder Fingerabdruck.</span><span class="sxs-lookup"><span data-stu-id="8108c-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="8108c-104">Wenn Sie die sichere Anmeldung wirklich deaktivieren möchten, lesen Sie die Anweisungen unter "Automatisches Anmelden bei Windows 10".</span><span class="sxs-lookup"><span data-stu-id="8108c-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="8108c-105">**Sichere Windows Hello-Alternativen zum Kontokennwort**</span><span class="sxs-lookup"><span data-stu-id="8108c-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="8108c-106">Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="8108c-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="8108c-107">Die verfügbaren Anmeldeoptionen werden aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="8108c-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="8108c-108">Beispiel:</span><span class="sxs-lookup"><span data-stu-id="8108c-108">For example:</span></span>

![Anmeldeoptionen.](media/sign-in-options.png)

<span data-ttu-id="8108c-110">Klicken oder tippen Sie auf eine der Optionen, um Sie zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="8108c-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="8108c-111">Wenn Sie das nächste Mal Windows starten oder entsperren, können Sie die neue Option anstelle eines Kennworts verwenden.</span><span class="sxs-lookup"><span data-stu-id="8108c-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="8108c-112">**Automatisches Anmelden bei Windows 10**</span><span class="sxs-lookup"><span data-stu-id="8108c-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="8108c-113">**Hinweis**: die automatische Anmeldung ist praktisch, führt jedoch ein Sicherheitsrisiko ein, insbesondere dann, wenn Ihr PC von mehreren Personen zugänglich ist.</span><span class="sxs-lookup"><span data-stu-id="8108c-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="8108c-114">Klicken oder tippen Sie auf die Schaltfläche **Start** in der Taskleiste.</span><span class="sxs-lookup"><span data-stu-id="8108c-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="8108c-115">Geben Sie **netplwiz** ein, und drücken Sie die EINGABETASTE, um das Fenster Benutzerkonten zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="8108c-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="8108c-116">Klicken Sie unter **Benutzerkonten**auf das Konto, für das Sie sich beim Start von Windows automatisch anmelden möchten.</span><span class="sxs-lookup"><span data-stu-id="8108c-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="8108c-117">Deaktivieren Sie das Kontrollkästchen "Benutzer müssen einen Benutzernamen und ein Kennwort für die Verwendung dieses Computers eingeben".</span><span class="sxs-lookup"><span data-stu-id="8108c-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Benutzer müssen eine Option für Benutzername und Kennwort eingeben.](media/users-must-enter-username.png)

5. <span data-ttu-id="8108c-119">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="8108c-119">Click **OK**.</span></span> <span data-ttu-id="8108c-120">Sie werden aufgefordert, das Kennwort für das ausgewählte Konto einzugeben und zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="8108c-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="8108c-121">Klicken Sie zum Abschließen auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="8108c-121">Click **OK** to finish.</span></span> <span data-ttu-id="8108c-122">Das nächste Mal, wenn Windows 10 gestartet wird, wird es sich automatisch bei dem ausgewählten Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="8108c-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
