---
title: Anmelden bei Windows 10 ohne Kennwort
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001690"
- "3766"
ms.openlocfilehash: 1c03f00f7b41ea16d3106b19b998edeea6114603
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830545"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a><span data-ttu-id="73c39-102">Anmelden bei Windows 10 ohne Kennwort</span><span class="sxs-lookup"><span data-stu-id="73c39-102">Sign-in to Windows 10 without using a password</span></span>

<span data-ttu-id="73c39-103">Um zu vermeiden, dass Sie beim Starten von Windows ein Kennwort eingeben müssen, empfehlen wir, eine der sicheren Anmeldeoptionen für Windows Hello zu verwenden, z. B. eine PIN, Gesichtserkennung oder Fingerabdruck, sofern verfügbar.</span><span class="sxs-lookup"><span data-stu-id="73c39-103">To avoid having to type a password at Windows startup, we recommend you use one of the Windows Hello secure sign-in options, like a PIN, face recognition, or fingerprint, if available.</span></span> <span data-ttu-id="73c39-104">Wenn Sie die sichere Anmeldung wirklich deaktivieren möchten, lesen Sie die Anweisungen "Automatische Anmeldung bei Windows 10" weiter unten.</span><span class="sxs-lookup"><span data-stu-id="73c39-104">If you really want to disable secure sign-in, see the "Automatically sign in to Windows 10" instructions below.</span></span>

<span data-ttu-id="73c39-105">**Sichern von Windows Hello-Alternativen zum Kontokennwort**</span><span class="sxs-lookup"><span data-stu-id="73c39-105">**Secure Windows Hello alternatives to the account password**</span></span>

<span data-ttu-id="73c39-106">Wechseln Sie **zu Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="73c39-106">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="73c39-107">Verfügbare Anmeldeoptionen werden aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="73c39-107">Available sign-in options will be listed.</span></span> <span data-ttu-id="73c39-108">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="73c39-108">For example:</span></span>

![Anmeldeoptionen.](media/sign-in-options.png)

<span data-ttu-id="73c39-110">Klicken oder tippen Sie auf eine der Optionen, um sie zu konfigurieren.</span><span class="sxs-lookup"><span data-stu-id="73c39-110">Click or tap one of the options to configure it.</span></span> <span data-ttu-id="73c39-111">Wenn Sie Windows das nächste Mal starten oder entsperren, können Sie die neue Option anstelle eines Kennworts verwenden.</span><span class="sxs-lookup"><span data-stu-id="73c39-111">Next time you start or unlock Windows, you will be able to use the new option instead of a password.</span></span> 

<span data-ttu-id="73c39-112">**Automatische Anmeldung bei Windows 10**</span><span class="sxs-lookup"><span data-stu-id="73c39-112">**Automatically sign-in to Windows 10**</span></span>

<span data-ttu-id="73c39-113">**Hinweis:** Die automatische Anmeldung ist praktisch, führt jedoch zu einem Sicherheitsrisiko, insbesondere wenn auf Ihren PC mehrere Personen zugriffen können.</span><span class="sxs-lookup"><span data-stu-id="73c39-113">**Note**: Automatic sign-in is convenient, but introduces a security risk, especially if your PC is accessible by multiple people.</span></span> 

1. <span data-ttu-id="73c39-114">Klicken oder tippen Sie **auf die Schaltfläche Start** in der Taskleiste.</span><span class="sxs-lookup"><span data-stu-id="73c39-114">Click or tap the **Start** button in the Taskbar.</span></span>

2. <span data-ttu-id="73c39-115">Geben **Sie netplwiz ein,** und drücken Sie die EINGABETASTE, um das Fenster Benutzerkonten zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="73c39-115">Type **netplwiz** and hit the Enter key to open the User Accounts window.</span></span>

3. <span data-ttu-id="73c39-116">Klicken **Sie unter Benutzerkonten** auf das Konto, bei dem Sie sich automatisch anmelden möchten, wenn Windows gestartet wird.</span><span class="sxs-lookup"><span data-stu-id="73c39-116">In **User Accounts**, click the account you want to automatically sign in to when Windows starts.</span></span>

4. <span data-ttu-id="73c39-117">Deaktivieren Sie das Kontrollkästchen "Benutzer müssen einen Benutzernamen und ein Kennwort eingeben, um diesen Computer zu verwenden".</span><span class="sxs-lookup"><span data-stu-id="73c39-117">Uncheck the "Users must enter a user name and password to use this computer" checkbox.</span></span>

    ![Benutzer müssen eine Benutzername- und Kennwortoption eingeben.](media/users-must-enter-username.png)

5. <span data-ttu-id="73c39-119">Klicken Sie auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="73c39-119">Click **OK**.</span></span> <span data-ttu-id="73c39-120">Sie werden aufgefordert, das Kennwort für das ausgewählte Konto einzugeben und zu bestätigen.</span><span class="sxs-lookup"><span data-stu-id="73c39-120">You will be asked to enter and confirm the password for the account you selected.</span></span> <span data-ttu-id="73c39-121">Klicken Sie zum Abschließen auf **OK**.</span><span class="sxs-lookup"><span data-stu-id="73c39-121">Click **OK** to finish.</span></span> <span data-ttu-id="73c39-122">Wenn Windows 10 das nächste Mal gestartet wird, wird es sich automatisch bei dem ausgewählten Konto anmelden.</span><span class="sxs-lookup"><span data-stu-id="73c39-122">Next time Windows 10 starts, it will automatically sign in to the account you selected.</span></span>
