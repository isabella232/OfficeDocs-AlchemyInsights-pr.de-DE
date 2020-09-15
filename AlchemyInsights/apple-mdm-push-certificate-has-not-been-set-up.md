---
title: Das Apple MDM-Push-Zertifikat wurde nicht eingerichtet
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716856"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="72d1c-102">Das Apple MDM-Push-Zertifikat wurde nicht eingerichtet</span><span class="sxs-lookup"><span data-stu-id="72d1c-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="72d1c-103">Ein Apple MDM-Push-Zertifikat (auch bekannt als Apple-Push-Benachrichtigungsdienst-Zertifikat (Apple Push Notification Service, APNS)) wurde nicht für Ihr Abonnement konfiguriert.</span><span class="sxs-lookup"><span data-stu-id="72d1c-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="72d1c-104">Ohne ein konfiguriertes Apple MDM-Push-Zertifikat, können Sie keine iOS-und Mac OS-Geräte registrieren und verwalten.</span><span class="sxs-lookup"><span data-stu-id="72d1c-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="72d1c-105">Nachdem Sie das Zertifikat zu Intune hinzugefügt haben, können Benutzer die Unternehmensportal-App installieren, um ihre iOS-Geräte zu registrieren.</span><span class="sxs-lookup"><span data-stu-id="72d1c-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="72d1c-106">Wählen Sie **Ich stimme zu** aus,</span><span class="sxs-lookup"><span data-stu-id="72d1c-106">Select **"I agree."**</span></span> <span data-ttu-id="72d1c-107">um Microsoft die Berechtigung zum Senden von Daten an Apple zu erteilen.</span><span class="sxs-lookup"><span data-stu-id="72d1c-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="72d1c-108">Wählen Sie **CSR herunterladen**, die Intune-Zertifikatsignieranforderung, die zum Erstellen eines Apple MDM-Push-Zertifikats erforderlich ist.</span><span class="sxs-lookup"><span data-stu-id="72d1c-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="72d1c-109">Die Datei wird verwendet, um ein Vertrauensstellungszertifikat vom Apple-Portal für Push-Zertifikate anzufordern.</span><span class="sxs-lookup"><span data-stu-id="72d1c-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="72d1c-110">Wählen Sie **Eigenes MDM-Push-Zertifikat erstellen** aus, um zum Apple-Portal für Push-Zertifikate zu wechseln.</span><span class="sxs-lookup"><span data-stu-id="72d1c-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="72d1c-111">Melden Sie sich mit der Apple-ID Ihres Unternehmens an, und wählen Sie dann **Zertifikat erstellen** aus.</span><span class="sxs-lookup"><span data-stu-id="72d1c-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="72d1c-112">Wählen Sie **Datei auswählen** aus, wechseln Sie zur Zertifikatsignieranforderungs-Datei, und wählen Sie dann **Hochladen** aus.</span><span class="sxs-lookup"><span data-stu-id="72d1c-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="72d1c-113">Wählen Sie auf der Seite „Bestätigung“ **Herunterladen** aus, um die Zertifikatdatei (.pem) herunterzuladen, und speichern Sie die Datei lokal.</span><span class="sxs-lookup"><span data-stu-id="72d1c-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="72d1c-114">**Hinweis**: Das Zertifikat ist der Apple-ID zugeordnet, mit der es erstellt wurde.</span><span class="sxs-lookup"><span data-stu-id="72d1c-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="72d1c-115">Verwenden Sie als bewährte Methode eine Apple-ID des Unternehmens für Verwaltungsaufgaben, und stellen Sie sicher, dass das Postfach von mehr als einer Person überwacht wird, oder indem Sie eine Verteilerliste verwenden.</span><span class="sxs-lookup"><span data-stu-id="72d1c-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="72d1c-116">Verwenden Sie niemals eine persönliche Apple-ID.</span><span class="sxs-lookup"><span data-stu-id="72d1c-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="72d1c-117">Verwenden Sie dieselbe Apple-ID, um das Apple-Push-Zertifikat alle 12 Monate zu verlängern.</span><span class="sxs-lookup"><span data-stu-id="72d1c-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="72d1c-118">Geben Sie die Apple-ID ein, mit der Sie Ihr Apple MDM-Push-Zertifikat erstellt haben.</span><span class="sxs-lookup"><span data-stu-id="72d1c-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="72d1c-119">Notieren Sie sich diese ID, damit Sie sie zur Hand haben, wenn Sie das Zertifikat verlängern müssen.</span><span class="sxs-lookup"><span data-stu-id="72d1c-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="72d1c-120">Wechseln Sie zur Zertifikatdatei (.pem), wählen Sie **Öffnen** aus, und wählen Sie dann **Hochladen** aus.</span><span class="sxs-lookup"><span data-stu-id="72d1c-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="72d1c-121">Mit dem Push-Zertifikat kann Intune Apple-Geräte registrieren und verwalten.</span><span class="sxs-lookup"><span data-stu-id="72d1c-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>