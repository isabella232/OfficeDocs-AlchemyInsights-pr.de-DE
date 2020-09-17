---
title: Verwenden von Fingerabdruck-Unlock-Option in Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795243"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="4a44e-102">Verwenden von Fingerabdruck-Unlock-Option in Windows 10</span><span class="sxs-lookup"><span data-stu-id="4a44e-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="4a44e-103">**Windows Hello-Fingerabdruck aktivieren**</span><span class="sxs-lookup"><span data-stu-id="4a44e-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="4a44e-104">Wenn Sie Windows 10 mit Ihrem Fingerabdruck entsperren möchten, müssen Sie Windows Hello Fingerprint einrichten, indem Sie mindestens einen Finger hinzufügen (sodass Windows erkennen kann, dass er Sie erkennt).</span><span class="sxs-lookup"><span data-stu-id="4a44e-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="4a44e-105">Wechseln Sie zu **Einstellungen > Konten > Anmeldeoptionen** (oder klicken Sie [hier](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="4a44e-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="4a44e-106">Die verfügbaren Anmeldeoptionen werden aufgelistet.</span><span class="sxs-lookup"><span data-stu-id="4a44e-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="4a44e-107">Zum Beispiel:</span><span class="sxs-lookup"><span data-stu-id="4a44e-107">For example:</span></span>

    ![Anmeldeoptionen.](media/sign-in-options.png)

2. <span data-ttu-id="4a44e-109">Klicken oder tippen Sie auf **Windows Hello Fingerprint**, und klicken Sie dann auf **Einrichten**.</span><span class="sxs-lookup"><span data-stu-id="4a44e-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="4a44e-110">Klicken Sie im Fenster Hello Setup von Windows auf **Erste Schritte**.</span><span class="sxs-lookup"><span data-stu-id="4a44e-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="4a44e-111">Der Fingerabdrucksensor wird aktiviert, und Sie werden aufgefordert, Ihren Finger auf den Sensor zu setzen:</span><span class="sxs-lookup"><span data-stu-id="4a44e-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Fingerabdrucksensor.](media/fingerprint-sensor.png)

3. <span data-ttu-id="4a44e-113">Befolgen Sie die Anweisungen, die Sie bitten, Ihren Finger wiederholt zu überprüfen.</span><span class="sxs-lookup"><span data-stu-id="4a44e-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="4a44e-114">Wenn dieser Vorgang abgeschlossen ist, haben Sie die Möglichkeit, weitere Finger hinzuzufügen, die Sie möglicherweise für die Anmeldung verwenden möchten.</span><span class="sxs-lookup"><span data-stu-id="4a44e-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="4a44e-115">Wenn Sie sich das nächste Mal bei Windows 10 anmelden, haben Sie die Möglichkeit, Ihren Fingerabdruck zu verwenden.</span><span class="sxs-lookup"><span data-stu-id="4a44e-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="4a44e-116">**Windows Hello Fingerabdruck nicht als Anmeldeoption verfügbar**</span><span class="sxs-lookup"><span data-stu-id="4a44e-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="4a44e-117">Wenn Windows Hello Fingerabdruck nicht als Option in den **Anmeldeoptionen**angezeigt wird, bedeutet dies, dass Windows keine Fingerabdruckleser/Scanner kennt, die an Ihren PC angeschlossen sind, oder dass eine Systemrichtlinie deren Verwendung verhindert (beispielsweise wenn Ihr PC von Ihrem Arbeitsplatz verwaltet wird).</span><span class="sxs-lookup"><span data-stu-id="4a44e-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="4a44e-118">Zur Problembehandlung:</span><span class="sxs-lookup"><span data-stu-id="4a44e-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="4a44e-119">Wählen Sie die Schaltfläche **Start** in der Taskleiste aus, und suchen Sie nach **Geräte-Manager**.</span><span class="sxs-lookup"><span data-stu-id="4a44e-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="4a44e-120">Klicken oder tippen Sie auf, um den **Geräte-Manager**zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="4a44e-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="4a44e-121">Erweitern Sie im Geräte-Manager biometrische Geräte, indem Sie auf dessen Chevron klicken.</span><span class="sxs-lookup"><span data-stu-id="4a44e-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Biometrische Geräte.](media/biometric-devices.png)

4. <span data-ttu-id="4a44e-123">Ihr Fingerabdruck-Scanner sollte als biometrisches Gerät wie der Synaptics WBDI-Scanner aufgeführt werden:</span><span class="sxs-lookup"><span data-stu-id="4a44e-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Biometrische Geräte.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="4a44e-125">Wenn Ihr Fingerabdruckscanner nicht angezeigt wird und der Scanner in Ihren PC integriert ist, wechseln Sie zur Website des PC-Herstellers.</span><span class="sxs-lookup"><span data-stu-id="4a44e-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="4a44e-126">Suchen Sie im Abschnitt technischer Support für Ihr PC-Modell nach einem Windows 10-Treiber für einen Scanner, den Sie installieren können.</span><span class="sxs-lookup"><span data-stu-id="4a44e-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="4a44e-127">Wenn der Scanner vom PC getrennt ist (über USB angeschlossen), wechseln Sie zur Website des Scanner-Herstellers, um die Gerätetreibersoftware von Windows 10 für das Scanner-Modell zu finden und zu installieren.</span><span class="sxs-lookup"><span data-stu-id="4a44e-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
