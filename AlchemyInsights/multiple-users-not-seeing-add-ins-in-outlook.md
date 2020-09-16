---
title: Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.openlocfilehash: a0c272f40044795754ed8630e88e00ed14ea6ad7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47729870"
---
# <a name="multiple-users-not-seeing-add-ins-in-outlook"></a>Mehreren Benutzern werden keine Add-Ins in Outlook angezeigt

Wenn Sie Outlook-Add-Ins testen und keine angezeigt werden, verwenden Sie als ersten Schritt zur Problembehandlung das PowerShell-Cmdlet **Get-OrganizationConfig**, um den Parameter _AppsForOffice Enabled_ abzufragen. Wenn die Abfrage den Wert **False** zurückgibt, setzen Sie diesen Parameter mit dem Cmdlet **Set-OrganizationConfig** auf **True**, damit Add-Ins wie erwartet angezeigt werden.

Es wird nicht empfohlen, den Parameter _AppsForOfficeEnabled_ auf **False** zu setzen. Der Wert **False**setzt alle vorstehenden Administrator- und Benutzerrolleneinstellungen außer Kraft und verhindert, dass neue Apps von einem Benutzer in der Organisation aktiviert werden.

Weitere Informationen finden Sie unter [Festlegen der Administratoren und Benutzer, die Add-Ins für Outlook installieren und verwalten dürfen](https://docs.microsoft.com/exchange/clients-and-mobile-in-exchange-online/add-ins-for-outlook/specify-who-can-install-and-manage-add-ins#user-roles).