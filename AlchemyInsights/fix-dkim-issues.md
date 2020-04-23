---
title: Beheben von Problemen mit DKIM-Setup
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1389
ms.assetid: ''
ms.openlocfilehash: d725eb0d46dcbf1b5b6d77ca9f59fcafa5298bf1
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 04/22/2020
ms.locfileid: "43717561"
---
# <a name="fix-dkim-setup-issues"></a><span data-ttu-id="356d2-102">Beheben von Problemen mit DKIM-Setup</span><span class="sxs-lookup"><span data-stu-id="356d2-102">Fix DKIM setup issues</span></span>

<span data-ttu-id="356d2-103">Wenn bei der Aktivierung von DKIM für Ihre benutzerdefinierte Domäne Probleme auftreten, führen Sie die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="356d2-103">If you experience issues enabling DKIM for your custom domain, use the following steps:</span></span>

- <span data-ttu-id="356d2-104">Die meisten DKIM-Setup Probleme beziehen sich auf falsche DNS-Einträge.</span><span class="sxs-lookup"><span data-stu-id="356d2-104">Most DKIM setup issues are related to incorrect DNS records.</span></span> <span data-ttu-id="356d2-105">Überprüfen Sie, ob der DKIM-CNAME-Eintrag (**kein** TXT-Eintrag) ordnungsgemäß formatiert ist.</span><span class="sxs-lookup"><span data-stu-id="356d2-105">Verify the DKIM CNAME record (**not** a TXT record) is formatted correctly.</span></span> <span data-ttu-id="356d2-106">Weitere Informationen finden Sie in diesem [Thema](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="356d2-106">For more information, see this [topic](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).</span></span>

- <span data-ttu-id="356d2-107">Nachdem Sie Ihre DKIM-DNS-Einträge beim DNS-Hostingdienst für Ihre Domäne (in der Regel Ihre Domänenregistrierungsstelle) erstellt oder aktualisiert haben, warten Sie, bis die DNS-Einträge weitergegeben werden.</span><span class="sxs-lookup"><span data-stu-id="356d2-107">After you create or update your DKIM DNS records at the DNS hosting service for your domain (typically, your domain registrar), wait for the DNS records to propagate.</span></span>

- <span data-ttu-id="356d2-108">Wenn Sie die DKIM-DNS-Einträge nicht im Admin Center erstellen können, können \<Sie\> CustomDomain durch Ihre benutzerdefinierte Domäne ersetzen (beispielsweise contoso.com) und diesen Befehl in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`ausführen.</span><span class="sxs-lookup"><span data-stu-id="356d2-108">If you can't create the DKIM DNS records in the admin center, you can replace \<CustomDomain\> with your custom domain (for example, contoso.com) and run this command in [Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell): `New-DkimSigningConfig -DomainName <CustomDomain> -Enabled $true`.</span></span>
