---
title: Verwalten der globalen Adressliste und des Offlineadressbuchs der Organisation
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022531"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="f7ef7-102">Verwalten der globalen Adressliste (GAL) und des Offlineadressbuchs (OAB) der Organisation</span><span class="sxs-lookup"><span data-stu-id="f7ef7-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="f7ef7-103">Bei einer globalen Adressliste (GAL) handelt es sich um eine Liste von E-Mail-aktivierten Objekten (beliebige Arten von E-Mail-Empfängern) in der Organisation.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="f7ef7-104">Eine GAL wird in jeder Organisation automatisch erstellt.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="f7ef7-105">Sie können weitere GALs erstellen, um Benutzer nach Organisation oder Standort zu trennen, aber ein einzelner Benutzer kann nur jeweils eine GAL sehen und verwenden.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="f7ef7-106">Einige E-Mail-Clients, z. B. Outlook für Windows, laden die GAL für die Offlinenutzung herunter.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="f7ef7-107">Dies wird als Offlineadressbuch (OAB) bezeichnet.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="f7ef7-108">In Exchange Online wird ein OAB nur einmal alle 8 Stunden aktualisiert, und dann muss es zum Aktualisieren der lokalen OAB-Kopie von den Clients heruntergeladen werden.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="f7ef7-109">Alle Empfängeränderungen müssen zuerst in der globalen Adressliste angezeigt werden, um sie später in ein OAB zu übernehmen.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="f7ef7-110">Hier sind einige häufig verwendete GAL- und OAB-Verfahren:</span><span class="sxs-lookup"><span data-stu-id="f7ef7-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="f7ef7-111">Aus einer Vielzahl von Gründen möchten Sie möglicherweise, dass einige Objekte in der globalen Adressliste verborgen sind.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="f7ef7-112">Weitere Informationen finden Sie unter [Ausblenden von Empfängern aus Adresslisten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="f7ef7-113">Wenn Sie bestimmten Benutzergruppen angepasste Ansichten der GAL der Organisation bereitstellen müssen, lesen Sie [Adressbuchrichtlinien in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="f7ef7-114">Informationen zum [Erstellen einer globalen Adressliste in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) und zum Arbeiten mit GAL-Berechtigungen finden Sie unter [Adresslisten in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="f7ef7-115">Beachten Sie, dass Sie, wenn Sie neue GALs erstellen, möglicherweise auch ein neues OAB erstellen sollten.</span><span class="sxs-lookup"><span data-stu-id="f7ef7-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="f7ef7-116">Siehe [Verfahren für Offlineadressbücher](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span><span class="sxs-lookup"><span data-stu-id="f7ef7-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
