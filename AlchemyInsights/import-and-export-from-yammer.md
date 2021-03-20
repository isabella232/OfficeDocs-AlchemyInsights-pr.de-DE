---
title: Importieren und Exportieren von Yammer
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
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897726"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="be92e-102">Importieren und Exportieren von Yammer</span><span class="sxs-lookup"><span data-stu-id="be92e-102">Import and export from Yammer</span></span>

<span data-ttu-id="be92e-103">**Importieren**</span><span class="sxs-lookup"><span data-stu-id="be92e-103">**Import**</span></span>

<span data-ttu-id="be92e-104">Die Optionen für den Benutzerimport variieren je nachdem, ob sich Ihr Yammer-Netzwerk im [Nativen Modus für Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode) befindet oder nicht.</span><span class="sxs-lookup"><span data-stu-id="be92e-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="be92e-105">**Nicht nativer Modus**: Benutzer können mithilfe der Option [Aus Adressbuch hinzufügen](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (maximal 100 Benutzer) in den Gruppeneinstellungen in Gruppen oder mithilfe der [Massenaktualisierung](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) innerhalb des Netzwerkadministrators in das Netzwerk importiert werden.</span><span class="sxs-lookup"><span data-stu-id="be92e-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="be92e-106">**Nativer Modus**: Gruppenmitgliedschafts- und Netzwerkmitgliedschaftsvorgänge sollten über das [Microsoft 365-Administratorportal](https://docs.microsoft.com/microsoft-365/admin/add-users), das [Azure AD-Portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory) oder mithilfe einer anderen Azure AD-Option ausgeführt werden.</span><span class="sxs-lookup"><span data-stu-id="be92e-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="be92e-107">Netzwerke im nativen Modus haben keinen Zugriff mehr auf Massenaktualisierungen und andere ältere Features.</span><span class="sxs-lookup"><span data-stu-id="be92e-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="be92e-108">Yammer hat das Importieren von Inhalten aus dem Netzwerkadministrator nie unterstützt, selbst wenn das Datenexportfeature in einem anderen Netzwerk verwendet wurde.</span><span class="sxs-lookup"><span data-stu-id="be92e-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="be92e-109">Inhalte können von Partnerlösungen oder den Yammer-REST-APIs erneut veröffentlicht werden.</span><span class="sxs-lookup"><span data-stu-id="be92e-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="be92e-110">**Export**</span><span class="sxs-lookup"><span data-stu-id="be92e-110">**Export**</span></span>

<span data-ttu-id="be92e-111">[Das Exportieren von Netzwerkdaten innerhalb von Netzwerkadministratoren](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) ermöglicht den Export von Inhalten aus Yammer-Netzwerken, einschließlich Nachrichten und Dateien.</span><span class="sxs-lookup"><span data-stu-id="be92e-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="be92e-112">Anhänge können sehr groß sein und dazu führen, dass der Export viel Zeit in Anspruch nimmt.</span><span class="sxs-lookup"><span data-stu-id="be92e-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="be92e-113">Wir empfehlen, aktive Netzwerke mithilfe der [Datenexport-API](https://developer.yammer.com/docs/data-export-api) in Blöcken nach Tag oder Woche zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="be92e-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="be92e-114">Der Microsoft-Support bietet zu diesem Zweck keine benutzerdefinierten Skripts an.</span><span class="sxs-lookup"><span data-stu-id="be92e-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="be92e-115">Es gibt einen separaten [GDPR-Export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise), um Inhalte für einen individuellen Benutzer zu exportieren.</span><span class="sxs-lookup"><span data-stu-id="be92e-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>