---
title: Konfigurieren des MIM Sync-Diensts
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430742"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="454ff-102">Konfigurieren des MIM Sync-Diensts</span><span class="sxs-lookup"><span data-stu-id="454ff-102">Configure MIM Sync service</span></span>

<span data-ttu-id="454ff-103">Der MIM-Synchronisierungsdienst (Microsoft Identity Manager) ist eine Komponente von MIM.</span><span class="sxs-lookup"><span data-stu-id="454ff-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="454ff-104">Es handelt sich um einen zentralisierten lokalen Dienst, der Informationen für Organisationen speichert und integriert, die über mehrere lokale Verzeichnisse und Datenbanken verfügen.</span><span class="sxs-lookup"><span data-stu-id="454ff-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="454ff-105">Möglicherweise können Sie Ihr Problem mit MIM Sync beheben, wenn die Ursache in einem aktuellen Update für MIM behoben wurde oder eines der anderen im folgenden Abschnitt genannten Probleme ist.</span><span class="sxs-lookup"><span data-stu-id="454ff-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="454ff-106">**Empfohlene Schritte**</span><span class="sxs-lookup"><span data-stu-id="454ff-106">**Recommended steps**</span></span>

1. <span data-ttu-id="454ff-107">Stellen Sie sicher, dass Sie ein aktuelles Update von MIM Sync verwenden, und prüfen Sie in den [MIM Sync-Versionshinweisen](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history), ob das Problem in einem Update behoben wurde.</span><span class="sxs-lookup"><span data-stu-id="454ff-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="454ff-108">Wenn das Problem mit dem Generic LDAP-, Generic SQL-, Lotus Domino- oder Web Services-Connector auftritt, stellen Sie sicher, dass Sie ein aktuelles Update der [generischen Connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history) verwenden.</span><span class="sxs-lookup"><span data-stu-id="454ff-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="454ff-109">Wenn eine MIM Sync-Ausführung mit einem Fehler abbricht, suchen Sie in der [Tabelle der Ausführungsfehlercodes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) nach den möglichen Ursachen.</span><span class="sxs-lookup"><span data-stu-id="454ff-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="454ff-110">Wenn die Ausführung mit **extension-dll-exception** abbricht, klicken Sie auf diese Worte, um das **Eigenschaftenfenster des Connectorbereichs** zu öffnen, und klicken Sie auf **Stapelüberwachung...**, um weitere Informationen über die zugrunde liegende Ursache zu erhalten, wie unter [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="454ff-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="454ff-111">Wenn die PCNS-Komponente (Password Change Notification Service) während der Kennwortsynchronisierung den **Fehler 6025** im Ereignisprotokoll meldet, lesen Sie die Anleitung zur Problembehandlung für [den Fehler 6025 in PCNS](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="454ff-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="454ff-112">Wenn die vollständige Synchronisierung mit dem FIM-Dienstverwaltungs-Agent langsam ist, überprüfen Sie die **auto grow**-Einstellung für TempDB, wie in [Problembehandlung bei der langsamen oder hängenden vollständigen Synchronisierung](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx) beschrieben.</span><span class="sxs-lookup"><span data-stu-id="454ff-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="454ff-113">Wenn ein stopped-server-Fehler mit „failed-creation-via-web-services“ bei Verwendung des FIM-Dienstverwaltungs-Agents auftritt, finden Sie unter [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) eine Übersicht über die Ursachen.</span><span class="sxs-lookup"><span data-stu-id="454ff-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

