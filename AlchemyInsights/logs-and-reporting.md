---
title: Protokolle und Berichterstellung
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031499"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="a85ae-102">Protokolle und Berichterstellung</span><span class="sxs-lookup"><span data-stu-id="a85ae-102">Logs and Reporting</span></span>

<span data-ttu-id="a85ae-103">[Häufig gestellte Fragen zur Azure Active](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) Directory-Berichterstellung beantwortet häufig gestellte Fragen zur Azure Active Directory (Azure AD)-Berichterstellung.</span><span class="sxs-lookup"><span data-stu-id="a85ae-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="a85ae-104">Weitere Informationen finden Sie in [der Azure Active Directory-Berichterstellung.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)</span><span class="sxs-lookup"><span data-stu-id="a85ae-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="a85ae-105">**Problembehandlung bei der Überwachung**</span><span class="sxs-lookup"><span data-stu-id="a85ae-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="a85ae-106">Wenn Sie Probleme mit einigen Überwachungsaktivitäten haben und die fehlende Aktivität in dieser Liste enthalten [ist,](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)geben Sie bitte ein Supportticket ein.</span><span class="sxs-lookup"><span data-stu-id="a85ae-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="a85ae-107">Wenn Probleme beim Anzeigen von Überwachungsprotokollen in Ihrem Mandanten auftreten, geben Sie ein Supportticket ein.</span><span class="sxs-lookup"><span data-stu-id="a85ae-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="a85ae-108">Wenn Ihre Überwachungsaktivitäten nicht sofort im Azure Portal [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) angezeigt werden, sehen Sie sich unsere Latenzinformationen an, und stellen Sie ein Supportticket ein, wenn die Verzögerung die dokumentierte Wartezeit überschreitet.</span><span class="sxs-lookup"><span data-stu-id="a85ae-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="a85ae-109">Aufbewahrung von Azure AD-Aktivitätsprotokollen</span><span class="sxs-lookup"><span data-stu-id="a85ae-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="a85ae-110">Wenn nicht alle Überwachungen für den ausgewählten Datumsbereich angezeigt werden, können Sie bis zu 250.000 Zeilen (sortiert nach den neuesten) Anmeldungen aus dem Azure-Portal herunterladen.</span><span class="sxs-lookup"><span data-stu-id="a85ae-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="a85ae-111">Weitere Informationen finden Sie unter [Herunterladen von Überwachungsaktivitäten.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)</span><span class="sxs-lookup"><span data-stu-id="a85ae-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="a85ae-112">**Problembehandlung bei Anmeldungen**</span><span class="sxs-lookup"><span data-stu-id="a85ae-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="a85ae-113">Sie können die Daten der letzten 30 Tage nur anzeigen, wenn Sie über eine Azure AD Premium (P1- oder P2)-Lizenz für Ihren Mandanten verfügen.</span><span class="sxs-lookup"><span data-stu-id="a85ae-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="a85ae-114">Anmeldungen sind nur für Azure AD Premium-Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a85ae-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="a85ae-115">Es ist nicht für kostenlose oder grundlegende lizenzierte Mandanten verfügbar.</span><span class="sxs-lookup"><span data-stu-id="a85ae-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="a85ae-116">Wenn Ihr Mandant über eine Premium -P1-Lizenz verfügt und [](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) Sie die Anmeldungen nicht sehen können, lesen Sie unsere Latenzinformationen, und stellen Sie ein Supportticket ein, wenn die Verzögerung die dokumentierte Latenz überschreitet.</span><span class="sxs-lookup"><span data-stu-id="a85ae-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="a85ae-117">Wenn nicht alle Anmeldungen für den ausgewählten Datumsbereich angezeigt werden, beachten Sie, dass Sie bis zu 250.000 Zeilen (sortiert nach der neuesten Version) von Anmeldungen aus dem Azure-Portal herunterladen können.</span><span class="sxs-lookup"><span data-stu-id="a85ae-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="a85ae-118">Weitere Informationen finden Sie unter [Herunterladen von Anmeldeaktivitäten.](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)</span><span class="sxs-lookup"><span data-stu-id="a85ae-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="a85ae-119">**Problembehandlung für Sicherheitsberichte (Gefährdete Benutzer, riskante Anmeldung)**</span><span class="sxs-lookup"><span data-stu-id="a85ae-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="a85ae-120">Benutzer, die für den Bericht zur Risikosicherheit gekennzeichnet sind</span><span class="sxs-lookup"><span data-stu-id="a85ae-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="a85ae-121">Bericht über riskante Anmeldungen im Azure Active Directory-Portal</span><span class="sxs-lookup"><span data-stu-id="a85ae-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="a85ae-122">Azure Active Directory-Risikoereignisse</span><span class="sxs-lookup"><span data-stu-id="a85ae-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
