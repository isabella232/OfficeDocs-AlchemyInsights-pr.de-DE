---
title: Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen
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
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 2f2d4f7c093d62267bb859e96493ec6d09452c7e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: de-DE
ms.lasthandoff: 09/14/2020
ms.locfileid: "47699518"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Aktualisieren von DNS-Einträgen, um die Website beim aktuellen Hostinganbieter zu belassen

1. Wechseln Sie im Microsoft 365 Admin Center zur Seite **Setup**  >  [Domänen](https://portal.office.com/adminportal/home#/Domains) , und wählen Sie in der Liste der Domänen die Domäne aus, die Sie für Ihre Website verwenden.

2. Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:

  - Geben Sie unter **DNS-Typ** ein: **A (Adresse)**

  - Geben Sie unter **Hostname oder Alias** Folgendes ein: **@**

  - Geben Sie unter **IP-Adresse** die statische IP-Adresse für Ihre Website ein, unter der diese derzeit gehostet wird, beispielsweise "172.16.140.1".

    Es muss eine  *statische*  IP-Adresse für die Website sein, keine  *dynamische*  . Überprüfen Sie bei der Website, auf der Ihre Website gehostet wird, dass Sie eine statische IP-Adresse für Ihre öffentliche Website erhalten können.

3. Klicken Sie auf **Speichern**.

Darüber hinaus können Sie einen CNAME-Eintrag erstellen, damit Kunden Ihre Website besser finden können.
  
1. Wählen Sie **+ Neuer benutzerdefinierter Eintrag** aus, und geben Sie Folgendes ein:

  - Geben Sie unter **DNS-Typ** ein: **CNAME (Alias)**

  - Geben Sie unter **Hostname oder Alias** Folgendes ein: **www**

  - Geben Sie unter **Verweist auf die Adresse** den vollqualifizierten Domänennamen (Fully Qualified Domain Name, FQDN) Ihrer Website ein, beispielsweise contoso.com.

2. Wählen Sie **Speichern**.
