---
title: Profilsynchronisierung
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923643"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Wann wird mein Profil mit der SharePoint Benutzerprofilanwendung synchronisiert?

SharePoint Online verwendet den Active Directory-Importzeitgeberauftrag (AD Import), um Benutzer und Gruppen in die Benutzerprofilanwendung zu importieren. 
  
1. Der AD-Import synchronisiert Änderungen aus dem SharePoint Onlineverzeichnis Store mit der Benutzerprofilanwendung. Diese Änderungen werden in Batches verarbeitet.
    
2. Der Zeitgeberauftrag wird ausgeführt, bis die Änderungen synchronisiert werden.
    
> [!NOTE]
> Wie lange der Auftrag ausgeführt werden muss, hängt von der Anzahl der zu verarbeitenden Änderungen ab. Eine große Anzahl von Änderungen dauert länger. Der Service Level Agreement (SLA) gibt an, dass eine Änderung an einem Benutzer im SharePoint Onlineverzeichnis in der Benutzerprofilanwendung in 24 Stunden widergespiegelt wird. 
  
[Weitere Informationen zur Benutzerprofilsynchronisierung in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

