---
title: Fixieren von Microsoft 365-apps konnten keine Office-Lizenzen finden. zugeordnete Nachricht
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3421"
- "9001426"
ms.openlocfilehash: bd127d6287b4438f6105a6158abdbd5b964b7e70
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47747694"
---
# <a name="fixing-the-microsoft-365-apps-couldnt-find-office-licenses-associated-message"></a>Beheben der Nachricht "Office-Lizenzen konnten nicht gefunden werden" für Microsoft 365-apps

Wenn Sie diese Meldung erhalten, versuchen Sie Folgendes:

1. Überprüfen Sie Ihre Firewall, Antivirensoftware und Proxyeinstellungen, um sicherzustellen, dass der Internet Zugriff auf Microsoft 365-apps nicht blockiert wird. Weitere Informationen finden Sie unter [Microsoft 365-URLs und IP-Adressbereiche](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).
2. Entfernen Sie [die Office-Lizenz](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) für den betroffenen Benutzer, und weisen Sie Sie neu zu. 
3. Öffnen Sie eine Office-App, und [melden Sie sich](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bei vorhandenen Benutzerkonten ab.
4. Wechseln Sie zu Windows-Einstellungen > **Konten**  >  **e-Mail-& Konten**, und entfernen Sie alle Arbeits Konten mit Ausnahme des betroffenen Kontos.
5. Wechseln Sie zu Windows-Einstellungen > **Konten**  >  **Zugriff auf Arbeit oder Schule**, und trennen Sie alle Arbeits Konten mit Ausnahme des betroffenen Kontos.
6. Setzen Sie den Office-Aktivierungsstatus zurück. [Anleitung](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).
7. [Melden Sie sich](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) mit dem betroffenen Benutzerkonto an.

Weitere Problem Behandlungslösungen finden Sie unter nicht [lizenziertes Produkt und Aktivierungsfehler in Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).