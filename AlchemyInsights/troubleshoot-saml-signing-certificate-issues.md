---
title: Behandeln von Problemen mit SAML-Signaturzertifikaten
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529211"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="35f1f-102">Behandeln von Problemen mit SAML-Signaturzertifikaten</span><span class="sxs-lookup"><span data-stu-id="35f1f-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="35f1f-103">Führen Sie die folgenden empfohlenen Schritte aus, um Probleme mit SAML-Signaturzertifikaten zu beheben:</span><span class="sxs-lookup"><span data-stu-id="35f1f-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="35f1f-104">Wenn Sie eine Unternehmensanwendung hinzufügen, die SSO (einmaliges Anmelden) unterstützt, generiert Azure ein Zertifikat, das als [SAML-Signaturzertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) bezeichnet wird.</span><span class="sxs-lookup"><span data-stu-id="35f1f-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="35f1f-105">Dieses Zertifikat hat eine Gültigkeit von 3 Jahren.</span><span class="sxs-lookup"><span data-stu-id="35f1f-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="35f1f-106">Informationen zum Ändern des Ablaufdatums Ihres Zertifikats finden Sie unter [Anpassen des Ablaufdatums eines Verbundzertifikats und dessen Rollup in ein neues Zertifikat](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span><span class="sxs-lookup"><span data-stu-id="35f1f-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="35f1f-107">Azure verwendet dieses Zertifikat, um die von der Anwendung angeforderten SAML-Token zu signieren und an die Anwendung für ein erfolgreiches einmaliges Anmelden (Single Sign-On, SSO) zu senden.</span><span class="sxs-lookup"><span data-stu-id="35f1f-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="35f1f-108">Damit dies durchgeführt werden kann, laden Sie das Zertifikat vom Azure-Portal herunter, und übermitteln Sie es an den Anwendungsanbieter, um den SSO-Prozess abzuschließen.</span><span class="sxs-lookup"><span data-stu-id="35f1f-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="35f1f-109">Nach Abschluss dieses Vorgangs vertraut die Anwendung diesem Zertifikat, und alle SAML-Token, die von diesem Zertifikat signiert sind, werden von ihr akzeptiert.</span><span class="sxs-lookup"><span data-stu-id="35f1f-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="35f1f-110">Wenn dieses Zertifikat abläuft, erstellen Sie ein neues, aktualisieren Sie es für den Anwendungsanbieter, und aktivieren Sie es dann auf Azure-Seite.</span><span class="sxs-lookup"><span data-stu-id="35f1f-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="35f1f-111">Weitere Informationen finden Sie unter [Erneuern eines Zertifikats, das in Kürze abläuft](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span><span class="sxs-lookup"><span data-stu-id="35f1f-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="35f1f-112">Wenn das Zertifikat abläuft, wird der Benutzer nicht blockiert.</span><span class="sxs-lookup"><span data-stu-id="35f1f-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="35f1f-113">[Fügen Sie eine E-Mail-Adresse für Benachrichtigung hinzu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration), die vor Ablauf des aktuellen Zertifikats versendet werden sollen.</span><span class="sxs-lookup"><span data-stu-id="35f1f-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="35f1f-114">Schritt 4 ist optional.</span><span class="sxs-lookup"><span data-stu-id="35f1f-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="35f1f-115">Ändern Sie die SAML-Zertifikatsignierungsoptionen einer Anwendung und den Zertifikatsignierungsalgorithmus.</span><span class="sxs-lookup"><span data-stu-id="35f1f-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="35f1f-116">Weitere Informationen finden Sie unter [Ändern von Zertifikatsignierungsoptionen und Signierungsalgorithmus](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span><span class="sxs-lookup"><span data-stu-id="35f1f-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

