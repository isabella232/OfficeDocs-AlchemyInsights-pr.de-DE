---
title: Moderne Azure-E-Mail-Rechnungsstellung
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003801"
- "6866"
ms.openlocfilehash: 65df6091a97d4937379ded384a78b5d07aa76e42
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 11/03/2020
ms.locfileid: "48840601"
---
# <a name="email-invoicing-in-azure"></a><span data-ttu-id="873dd-102">E-Mail-Rechnungsstellung in Azure</span><span class="sxs-lookup"><span data-stu-id="873dd-102">Email invoicing in Azure</span></span>

<span data-ttu-id="873dd-103">Sie müssen über die Rolle "Besitzer" oder "Mitwirkender" für das Abrechnungsprofil oder das entsprechende Abrechnungskonto verfügen, um die Einstellungen für E-Mail-Rechnungen aktualisieren zu können.</span><span class="sxs-lookup"><span data-stu-id="873dd-103">You must have an owner or a contributor role on the billing profile or its billing account to update its email invoice preference.</span></span> <span data-ttu-id="873dd-104">Nach der Aktivierung erhalten alle Benutzer mit der Rolle "Besitzer", "Mitwirkender", "Leser" und "Rechnungsadministrator" die Rechnung per E-Mail.</span><span class="sxs-lookup"><span data-stu-id="873dd-104">Once you have opted-in, all users with an owner, contributor, readers, and invoice manager roles on a billing profile will get its invoice in email.</span></span>

1. <span data-ttu-id="873dd-105">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="873dd-105">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="873dd-106">Suchen Sie nach **Kostenverwaltung und Abrechnung**.</span><span class="sxs-lookup"><span data-stu-id="873dd-106">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="873dd-107">Wählen Sie auf der linken Seite **Rechnungen** und dann oben auf der Seite **E-Mail-Rechnung** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-107">Select **Invoices** from the left-hand side and then select **Email Invoice** from the top of the page.</span></span>
4. <span data-ttu-id="873dd-108">Wenn Sie über mehrere Abrechnungsprofile verfügen, wählen Sie das gewünschte Abrechnungsprofil und dann **Aktivieren** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-108">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

5. <span data-ttu-id="873dd-109">Wählen Sie **Aktualisieren** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-109">Select **Update**.</span></span>
6. <span data-ttu-id="873dd-110">Wenn Sie über mehrere Abrechnungsprofile verfügen, wählen Sie das gewünschte Abrechnungsprofil und dann **Aktivieren** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-110">If you have multiple billing profiles, select a billing profile and then select **Opt in**.</span></span>

<span data-ttu-id="873dd-111">Sie können anderen Personen das Anzeigen, Herunterladen und Begleichen von Rechnungen gestatten, indem Sie ihnen die Rolle "Rechnungsadministrator" für ein MCA- oder MPA-Abrechnungsprofil zuweisen.</span><span class="sxs-lookup"><span data-stu-id="873dd-111">You give others access to view, download, and pay invoices by assigning them the invoice manager role for an MCA or MPA billing profile.</span></span> <span data-ttu-id="873dd-112">Wenn Sie den Erhalt von Rechnungen per E-Mail aktiviert haben, erhalten die Benutzer die Rechnungen ebenfalls per E-Mail.</span><span class="sxs-lookup"><span data-stu-id="873dd-112">If you've opted in to get your invoice in email, users also get the invoices in email.</span></span>

1. <span data-ttu-id="873dd-113">Melden Sie sich beim [Azure-Portal](https://portal.azure.com/) an.</span><span class="sxs-lookup"><span data-stu-id="873dd-113">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="873dd-114">Suchen Sie nach **Kostenverwaltung und Abrechnung**.</span><span class="sxs-lookup"><span data-stu-id="873dd-114">Search for **Cost Management + Billing**.</span></span>
3. <span data-ttu-id="873dd-115">Wählen Sie auf der linken Seite **Abrechnungsprofile** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-115">Select **Billing profiles** from the left-hand side.</span></span> <span data-ttu-id="873dd-116">Wählen Sie in der Liste der Abrechnungsprofile jenes aus, für das Sie jemandem die Rolle "Rechnungsadministrator" zuweisen möchten.</span><span class="sxs-lookup"><span data-stu-id="873dd-116">From the billing profiles list, select a billing profile for which you want to assign an invoice manager role.</span></span>
4. <span data-ttu-id="873dd-117">Wählen Sie auf der linken Seite **Zugriffssteuerung (IAM)** und dann oben auf der Seite **Hinzufügen** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-117">Select **Access Control (IAM)** from the left-hand side and then select **Add** from the top of the page.</span></span>

<span data-ttu-id="873dd-118">Wählen Sie in der Dropdownliste der Rollen **Rechnungsadministrator** aus.</span><span class="sxs-lookup"><span data-stu-id="873dd-118">In the Role drop-down list, select **Invoice Manager**.</span></span> <span data-ttu-id="873dd-119">Geben Sie die E-Mail-Adresse des Benutzers ein, der Zugriff erhalten soll.</span><span class="sxs-lookup"><span data-stu-id="873dd-119">Enter the email address of the user to give access.</span></span> <span data-ttu-id="873dd-120">Wählen Sie **Speichern** aus, damit die Rolle zugewiesen wird.</span><span class="sxs-lookup"><span data-stu-id="873dd-120">Select **Save** to assign the role.</span></span>
