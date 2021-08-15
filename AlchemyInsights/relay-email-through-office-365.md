---
title: Weiterleiten von E-Mails über Microsoft 365
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "154"
- "3000003"
ms.assetid: 84191e23-496c-495a-a2ec-28c5ae0d4c0b
ms.openlocfilehash: ef06cfe41eee5d67bf82d4f64875ddafac82ee2062aade761f81b906cd428dd5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "54024205"
---
# <a name="set-up-a-multifunction-device-or-application-to-send-email"></a>Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails

Weitere Informationen zu den verfügbaren Optionen und erforderlichen Schritten finden Sie unter [Einrichten eines Multifunktionsgeräts oder einer Anwendung zum Senden von E-Mails mithilfe von Microsoft 365](/Exchange/mail-flow-best-practices/how-to-set-up-a-multifunction-device-or-application-to-send-email-using-microsoft-365-or-office-365).
  
Wenn Sie ein Gerät oder eine Anwendung haben, das/die seit Kurzem nicht mehr funktioniert, sind die häufigsten Probleme:

- **Authentifizierungsbezogene Fehler bei der Verwendung der SMTP-Authentifizierungsclientübermittlung** Wir haben vor Kurzem einige Änderungen an der Funktionsweise der SMTP-Authentifizierung vorgenommen. Weitere Informationen zum Beheben von Problemen finden Sie im Abschnitt "Authentifizierung nicht erfolgreich" unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mit Microsoft 365 oder Office 365 senden](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off#error-authentication-unsuccessful).
- **Wir akzeptieren nur die TLS 1.2-Version, während eine sichere Verbindung zu Office 365 hergestellt wird** Wenn Sie eine sichere Verbindung (TLS) verwenden, stellen Sie sicher, dass Ihr Anwendungsgerät TLS 1.2 unterstützt. Weitere Informationen finden Sie unter [Vorbereiten für TLS 1.2 in Office 365 und Office 365 GCC](/microsoft-365/compliance/prepare-tls-1.2-in-office-365).
 
Weitere Probleme und Lösungen finden Sie unter [Beheben von Problemen mit Druckern, Scannern und Branchenanwendungen, die E-Mails mithilfe von Microsoft 365 oder Office 365 senden](/Exchange/mail-flow-best-practices/fix-issues-with-printers-scanners-and-lob-applications-that-send-email-using-off).

Um betroffene Geräte anzuzeigen, wechseln Sie zum [SMTP Auth-Clientsbericht](https://protection.office.com/mailflow/dashboard).

**Hinweis**: Exchange Online unterstützt keine Massensendungsszenarien. Um kommerzielle Massen-E-Mails (z. B. Kunden-Newsletter) zu versenden, sollten Sie Drittanbieter verwenden, die auf diese Dienste spezialisiert sind.
