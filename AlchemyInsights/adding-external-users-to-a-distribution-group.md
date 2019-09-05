---
title: Hinzufügen externer Benutzer zu einer Verteilergruppe
ms.author: chrisda
author: chrisda
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: caa0f310-0bb7-48e3-8ad2-cb358b53bbba
ms.openlocfilehash: e84a5b04d6fc805deaa47cb10c91081f37411e5b
ms.sourcegitcommit: a256e8680379c006287ae30996763051c4d9ff85
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/04/2019
ms.locfileid: "36737872"
---
# <a name="add-external-users-to-a-distribution-group"></a><span data-ttu-id="93462-102">Hinzufügen externer Benutzer zu einer Verteilergruppe</span><span class="sxs-lookup"><span data-stu-id="93462-102">Add external users to a Distribution Group</span></span>

<span data-ttu-id="93462-103">Das Hinzufügen eines externen Kontakts zu einer Verteilergruppe (DG) ist ein zweistufiger Prozess:</span><span class="sxs-lookup"><span data-stu-id="93462-103">Adding an external contact to a Distribution Group (DG) is a two-step process:</span></span>
  
1. <span data-ttu-id="93462-104">Erstellen Sie einen e-Mail-Kontakt für den externen Benutzer:</span><span class="sxs-lookup"><span data-stu-id="93462-104">Create a Mail Contact for the external user:</span></span>
    
    1. <span data-ttu-id="93462-105">Wechseln Sie im Admin Center zur Seite **Benutzer** > [Kontakte](https://admin.microsoft.com/adminportal/home#/Contact) .</span><span class="sxs-lookup"><span data-stu-id="93462-105">In the admin center, go to the **Users** > [Contacts](https://admin.microsoft.com/adminportal/home#/Contact) page.</span></span> 
    
    2. <span data-ttu-id="93462-106">Wählen Sie **Kontakt hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="93462-106">Select **Add a contact**.</span></span>
    
    3. <span data-ttu-id="93462-107">Geben Sie die Informationen für Ihren Kontakt ein, und wählen Sie **Hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="93462-107">Type the information for your contact and select **Add**.</span></span>
    
2. <span data-ttu-id="93462-108">Fügen Sie den e-Mail-Kontakt zu Ihrer GD hinzu:</span><span class="sxs-lookup"><span data-stu-id="93462-108">Add the Mail Contact to your DG:</span></span>
    
    1. <span data-ttu-id="93462-109">Wechseln Sie im Admin Center zur Seite **Gruppen** > [Gruppen.](https://admin.microsoft.com/adminportal/home#/groups)</span><span class="sxs-lookup"><span data-stu-id="93462-109">In the admin center, go to the **Groups** > [Groups](https://admin.microsoft.com/adminportal/home#/groups) page.</span></span> 
    
    2. <span data-ttu-id="93462-110">Suchen Sie die GD, der Sie den externen Benutzer hinzufügen möchten, und wählen Sie Sie aus, um das Dialogfeld bearbeiten zu öffnen.</span><span class="sxs-lookup"><span data-stu-id="93462-110">Find the DG you want to add the external user to, and select it to open the edit dialog.</span></span>
    
    3. <span data-ttu-id="93462-111">Wählen Sie auf der Registerkarte **Mitglieder** die Option **Alle anzeigen und Mitglieder verwalten**aus.</span><span class="sxs-lookup"><span data-stu-id="93462-111">On the **Members** tab, select **View all and manage members**.</span></span> 
    
    4. <span data-ttu-id="93462-112">Wählen Sie **Mitglieder hinzufügen**aus.</span><span class="sxs-lookup"><span data-stu-id="93462-112">Select **Add members**.</span></span>
    
    5. <span data-ttu-id="93462-113">Wählen Sie den e-Mail-Kontakt aus, den Sie im vorherigen Schritt erstellt haben, und wählen Sie dann **Speichern**aus.</span><span class="sxs-lookup"><span data-stu-id="93462-113">Select the Mail Contact you created on the previous step, and then select **Save**.</span></span>
    
<span data-ttu-id="93462-114">Wenn Ihre externen Benutzer nach diesen Schritten keine e-Mails an die DG senden können oder keine e-Mails davon erhalten, kann es sein, dass die DG so gekennzeichnet ist, dass Sie nur e-Mails von internen Benutzern zulässt.</span><span class="sxs-lookup"><span data-stu-id="93462-114">If after following these steps your external users can't send emails to the DG or don't receive emails from it, it could be that the DG is marked to only allow emails from internal users.</span></span> <span data-ttu-id="93462-115">Sie können diese Konfiguration überprüfen und nach den Anweisungen [hier](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online)korrigieren.</span><span class="sxs-lookup"><span data-stu-id="93462-115">You can check this configuration and fix it following the directions [here](https://docs.microsoft.com/exchange/mail-flow-best-practices/non-delivery-reports-in-exchange-online/fix-error-code-5-7-133-in-exchange-online).</span></span>
  
 <span data-ttu-id="93462-116">**Hinweis:** Diese Anweisungen gelten nicht, wenn der Typ der Gruppe "Office 365 Gruppe" anstelle von "Verteilergruppe" lautet.</span><span class="sxs-lookup"><span data-stu-id="93462-116">**Note:** These instructions don't apply if your group's type is "Office 365 group" instead of "Distribution group."</span></span> <span data-ttu-id="93462-117">Wenn dies der Fall ist, können Sie den externen Benutzer direkt aus Outlook zur Gruppe hinzufügen.</span><span class="sxs-lookup"><span data-stu-id="93462-117">If that is the case, you can add the external user directly to the group from Outlook.</span></span> <span data-ttu-id="93462-118">Ausführliche Informationen zu Office 365 Gruppen sowie Anweisungen zum Hinzufügen externer Gäste finden Sie in [diesem Artikel](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span><span class="sxs-lookup"><span data-stu-id="93462-118">Detailed information on Office 365 groups guests as well as instructions for adding external guests can be found in [this article](https://support.office.com/article/Guest-access-in-Office-365-Groups-bfc7a840-868f-4fd6-a390-f347bf51aff6.aspx).</span></span>
  