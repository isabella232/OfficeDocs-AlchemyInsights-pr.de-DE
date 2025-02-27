---
title: Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334384"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>Das Benutzerbild erscheint weiterhin im Microsoft Teams Organigramm

Wenn eine oder mehrere Personen in Ihrer Organisation deaktiviert oder entfernt wurden und ihr Profilfoto weiterhin im Organigramm angezeigt wird, ist es möglich, dass die Einstellung **"ShowInAddressLists"** auf "False" festgelegt ist: 

1. Wechseln Sie zu Microsoft 365 Admin Center > [Aktive Benutzer](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users) und wählen Sie den Benutzer mit dem Foto aus, das weiter angezeigt wird. 
1. Wählen Sie die Registerkarte **E-Mail** aus, und stellen Sie sicher, dass **in der globalen Adressliste anzeigen** auf **Nein** festgelegt ist.

Wenn das Festlegen von **ShowInAddressLists** auf **Nein** nicht funktioniert, überprüfen Sie Folgendes: 

- Der Benutzer wird möglicherweise aus der Empfängerliste in Exchange angezeigt. Weitere Informationen finden Sie unter [Adressliste in Exchange Online verwalten](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists). 
- Der Benutzer wird möglicherweise aus der Adressenliste in Azure Active Directory angezeigt. Weitere Informationen finden Sie unter [Set-AzureADUser](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0). 