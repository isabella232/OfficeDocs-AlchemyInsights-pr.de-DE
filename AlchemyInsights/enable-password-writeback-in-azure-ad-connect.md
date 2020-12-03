---
title: Aktivieren des Kennwortrückschreibens in Azure AD Connect
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
- "9002933"
- "5615"
ms.openlocfilehash: 0eecd89b2558359702935379d7ffbd8b7508f4cd
ms.sourcegitcommit: 62a83a1c6bd9779a1a11b749490bd11670d4b063
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 12/02/2020
ms.locfileid: "49560439"
---
# <a name="enable-password-writeback-in-azure-ad-connect"></a><span data-ttu-id="46b90-102">Aktivieren des Kennwortrückschreibens in Azure AD Connect</span><span class="sxs-lookup"><span data-stu-id="46b90-102">Enable password writeback in Azure AD Connect</span></span>

<span data-ttu-id="46b90-103">Wenn Sie das Rückschreiben für die Self-Service-Kennwortzurücksetzung aktivieren möchten, aktivieren Sie zuerst die Rückschreibeoption in Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="46b90-103">To enable self-service password reset writeback, first enable the writeback option in Azure AD Connect.</span></span> <span data-ttu-id="46b90-104">Führen Sie auf Ihrem Azure AD Connect-Server die folgenden Schritte aus:</span><span class="sxs-lookup"><span data-stu-id="46b90-104">From your Azure AD Connect server, complete the following steps:</span></span>

1. <span data-ttu-id="46b90-105">Melden Sie sich bei Ihrem Azure AD Connect-Server an, und starten Sie den Konfigurations-Assistenten **Azure AD Connect**.</span><span class="sxs-lookup"><span data-stu-id="46b90-105">Sign in to your Azure AD Connect server and start the **Azure AD Connect** configuration wizard.</span></span>
2. <span data-ttu-id="46b90-106">Klicken Sie auf der **Begrüßungsseite** auf **Konfigurieren**.</span><span class="sxs-lookup"><span data-stu-id="46b90-106">On the **Welcome** page, click **Configure**.</span></span>
3. <span data-ttu-id="46b90-107">Wählen Sie auf dem Seite **Weitere Aufgaben** die Option **Synchronisierungsoptionen anpassen** aus, und klicken Sie dann auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="46b90-107">On the **Additional tasks** page, select **Customize synchronization options**, and then click **Next**.</span></span>
4. <span data-ttu-id="46b90-108">Geben Sie auf der Seite **Mit Azure AD verbinden** die Anmeldeinformationen für Ihren Azure-Mandanten ein, und klicken Sie dann auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="46b90-108">On the **Connect to Azure AD** page, enter a global administrator credential for your Azure tenant, and then click **Next**.</span></span>
5. <span data-ttu-id="46b90-109">Klicken sie auf den Filterseiten **Verzeichnisse verbinden** und **Domänen/OE** auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="46b90-109">On the **Connect directories** and **Domain/OU** filtering pages, click **Next**.</span></span>
6. <span data-ttu-id="46b90-110">Wählen Sie auf der Seite **Optionale Funktionen** das Kästchen neben **Kennwortrückschreiben** aus, und klicken Sie dann auf **Weiter**.</span><span class="sxs-lookup"><span data-stu-id="46b90-110">On the **Optional features** page, select the box next to **Password writeback** and click **Next**.</span></span>
7. <span data-ttu-id="46b90-111">Klicken Sie auf der Seite **Bereit zum Konfigurieren** auf **Konfigurieren** und warten Sie, bis der Vorgang abgeschlossen ist.</span><span class="sxs-lookup"><span data-stu-id="46b90-111">On the **Ready to configure** page, click **Configure** and wait for the process to finish.</span></span>
8. <span data-ttu-id="46b90-112">Wenn die Option zum Abschließen der Konfiguration angezeigt wird, klicken Sie auf **Beenden**.</span><span class="sxs-lookup"><span data-stu-id="46b90-112">When you see the configuration finish, click **Exit**.</span></span>

<span data-ttu-id="46b90-113">Wenn das Kennwortrückschreiben in Azure AD Connect aktiviert ist, konfigurieren Sie Azure AD SSPR für das Rückschreiben.</span><span class="sxs-lookup"><span data-stu-id="46b90-113">With password writeback enabled in Azure AD Connect, configure Azure AD SSPR for writeback.</span></span>  <span data-ttu-id="46b90-114">Führen Sie die folgenden Schritte aus, um das Kennwortrückschreiben in SSPR zu aktivieren:</span><span class="sxs-lookup"><span data-stu-id="46b90-114">To enable password writeback in SSPR, complete the following steps:</span></span>

1. <span data-ttu-id="46b90-115">Melden Sie sich mit einem globalen Administratorkonto beim Azure-Portal an.</span><span class="sxs-lookup"><span data-stu-id="46b90-115">Sign in to the Azure portal using a global administrator account.</span></span>
2. <span data-ttu-id="46b90-116">Suchen Sie nach **Azure Active Directory**, wählen Sie es aus, klicken Sie auf **Kennwortzurücksetzung** und dann auf **Lokale Integration**.</span><span class="sxs-lookup"><span data-stu-id="46b90-116">Search for and select **Azure Active Directory**, click **Password reset**, then click **On-premises integration**.</span></span>
3. <span data-ttu-id="46b90-117">Legen Sie die Option für **Kennwörter in Ihr lokales Verzeichnis zurückschreiben?** auf **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="46b90-117">Set the option for **Write back passwords to your on-premises directory?** to **Yes**.</span></span>
4. <span data-ttu-id="46b90-118">Legen Sie die Option für **Zulassen, dass Benutzer Konten entsperren können, ohne das Kennwort zurückzusetzen?** auf **Ja** fest.</span><span class="sxs-lookup"><span data-stu-id="46b90-118">Set the option for **Allow users to unlock accounts without resetting their password?** to **Yes**.</span></span>
5. <span data-ttu-id="46b90-119">Klicken Sie abschließend auf **Speichern**.</span><span class="sxs-lookup"><span data-stu-id="46b90-119">When ready, click **Save**.</span></span>

<span data-ttu-id="46b90-120">Weitere Informationen finden Sie unter [Aktivieren des Zurückschreibens einer Azure Active Directory Self-Service-Kennwortzurücksetzung in eine lokale Umgebung](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span><span class="sxs-lookup"><span data-stu-id="46b90-120">For more information, see [Enable Azure Active Directory self-service password reset writeback to an on-premises environment](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr-writeback).</span></span>

> [!NOTE]
>  <span data-ttu-id="46b90-121">Setzt ein Administrator das Kennwort eines Benutzers im Azure-Portal zurück, wird das Kennwort in das lokale System zurückgeschrieben, wenn dieser Benutzer ein Verbundbenutzer ist oder mit einem Kennworthash synchronisiert wird.</span><span class="sxs-lookup"><span data-stu-id="46b90-121">When an administrator resets a user's password in the Azure Portal, if that user is federated or password hash synchronized, the password is written back to on-premises.</span></span> <span data-ttu-id="46b90-122">Diese Funktionalität wird derzeit im Office-Administratorportal nicht unterstützt.</span><span class="sxs-lookup"><span data-stu-id="46b90-122">This functionality is currently not supported in the Office Admin portal.</span></span>