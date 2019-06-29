---
title: 929 Posteingangsregeln zu deflectTransport Regeln
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6cf996e6d0a2698a5ce2bb57251de7c61d248d2a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 06/28/2019
ms.locfileid: "35382664"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="b61a6-102">Nachrichtenfluss Regeln (auch als Transportregeln bezeichnet)</span><span class="sxs-lookup"><span data-stu-id="b61a6-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="b61a6-103">Allgemeine Übersicht über Nachrichtenfluss Regeln: [Nachrichtenfluss Regeln (Transportregeln) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="b61a6-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="b61a6-104">Einrichten von Nachrichtenfluss Regeln: [Nachrichtenfluss Regelverfahren in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="b61a6-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="b61a6-105">Erstellen, ändern und Löschen von Nachrichtenfluss Regeln: [Verwalten von Nachrichtenfluss Regeln](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="b61a6-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="b61a6-106">Sie können auch Nachrichtenfluss Regeln in Exchange Online PowerShell verwalten.</span><span class="sxs-lookup"><span data-stu-id="b61a6-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="b61a6-107">Weitere Informationen finden Sie unter [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (View), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (Create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [Sets-](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) TransportRule (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (Disable existing) und [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (vorhandene aktivieren).</span><span class="sxs-lookup"><span data-stu-id="b61a6-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="b61a6-108">Zusätzliche Cmdlets für Nachrichtenfluss Regeln: [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) Action (List Available Actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (Auflisten der verfügbaren Bedingungen und Ausnahmen), [Export-](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) TransportRuleCollection (Export Rules) und [ Import-](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) TransportRuleCollection (Import Rules).</span><span class="sxs-lookup"><span data-stu-id="b61a6-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
