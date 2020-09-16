---
title: Verschlüsselung mit Transportregeln
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
- "9002635"
- "5154"
ms.openlocfilehash: 4c43fc16db84832c4e2aa3b6483632de6861b877
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 09/15/2020
ms.locfileid: "47784342"
---
# <a name="encryption-with-transport-rules"></a>Verschlüsselung mit Transportregeln

Im [Exchange Admin Center](https://go.microsoft.com/fwlink/p/?linkid=834822) (EAC) können Sie die Funktionen der Office-Nachrichtenverschlüsselung (OME) in ihren Nachrichtenflussregeln verwenden, um die Nachrichtenverschlüsselung auszulösen. Wählen Sie die Option **Office 365-Nachrichtenverschlüsselung und Rechteschutz** in der Transportregelbedingung aus.

- Weitere Informationen finden Sie unter [Definieren von Nachrichtenflussregeln zum Verschlüsseln von E-Mails](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email).

- Verwenden Sie in PowerShell das Cmdlet [New-TransportRule](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email?view=o365-worldwide#use-exchange-online-powershell-to-create-a-mail-flow-rule-for-encrypting-email-messages-without-the-new-ome-capabilities), und legen Sie den Parameter *ApplyOME* auf "$true" fest.
