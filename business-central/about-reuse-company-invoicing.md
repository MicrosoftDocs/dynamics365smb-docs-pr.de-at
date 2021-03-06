---
title: Invoicing und Business Central verwenden | Microsoft Docs
description: Problemumgehung für den Zugriff auf Microsoft Invoicing, wenn Sie sich für Dynamics 365 Business Central registriert haben.
author: bholtorf
ms.service: dynamics365-business-central
ms.topic: article
ms.devlang: na
ms.tgt_pltfrm: na
ms.workload: na
ms.search.keywords: Invoicing, Microsoft 365
ms.date: 10/01/2020
ms.author: bholtorf
ms.openlocfilehash: 4267dfb550fb4e8ccf2181762b2b5edcbd0fc188
ms.sourcegitcommit: 2e7307fbe1eb3b34d0ad9356226a19409054a402
ms.translationtype: HT
ms.contentlocale: de-AT
ms.lasthandoff: 12/17/2020
ms.locfileid: "4753584"
---
# <a name="using-the-same-microsoft-365-account-in-prod_short-and-microsoft-invoicing"></a>Verwenden des gleichen Microsoft 365-Kontos in [!INCLUDE[prod_short](includes/prod_long.md)] und Microsoft Invoicing
Wenn Sie sich für eine Testversion anmelden [!INCLUDE[prod_short](includes/prod_short.md)], können das Programm 30-Tage lang testen, Sie können ein Abonnement abschließen oder Sie können die Verwendung von [!INCLUDE[prod_short](includes/prod_short.md)] beenden. In allen Fällen wurde möglicherweise irgendwann **Microsoft Invoicing** angezeigt und Sie haben darauf geklickt. Dies war eine App, die Teil des heutigen Microsoft 365 Business Standard war und früher als Microsoft 365 Business Premium-Abonnement bezeichnet wurde, sodass diese Kachel nicht in jeder Microsoft 365-Umgebung angezeigt wurde.  

Microsoft Invoicing ist nicht mehr verfügbar. Wenn Sie sich jedoch bei Invoicing anmelden müssen, um Ihre Daten abzurufen, wird möglicherweise die Meldung angezeigt, dass Sie nicht auf Microsoft Invoicing zugreifen können, da Ihr Konto in [!INCLUDE[prod_short](includes/prod_short.md)] verwendet wird.  

Sie sehen eine ähnliche Meldung, wenn Sie die mobile App für die Fakturierung einrichten.  

## <a name="workaround"></a>Problemumgehung
Invoicing und [!INCLUDE[prod_short](includes/prod_short.md)] haben eine freigegebene Plattform. Das bedeutet, dass Sie als bestehender Benutzer von [!INCLUDE[prod_short](includes/prod_short.md)] erkannt werden, wenn Sie auf Rechnungsstellung im Microsoft 365 Admin Center klicken. Der Grund ist, dass das Invoicing nicht das gleiche Unternehmen als [!INCLUDE[prod_short](includes/prod_short.md)] verwenden kann.  

Daher müssen Sie sich bei [!INCLUDE[prod_short](includes/prod_short.md)] anmelden und Ihr bestehendes Unternehmen umbenennen und dann ein neues Unternehmen erstellen, dass Sie dann in Invoicing verwenden können. Keine Daten werden bei dieser Problemumgehung überschrieben oder verschoben.

### <a name="to-rename-your-company"></a>Ihr Unternehmen umbenennen
1. Melden Sie sich an bei [!INCLUDE[prod_short](includes/prod_short.md)].
2. Wählen Sie in der oberen rechten Ecke das Symbol **Einstellungen** ![Einstellungen](media/ui-experience/settings_icon_small.png "Einstellungssymbol für Rollencenter") und dann **Meine Einstellungen**.
3. Wählen Sie im Feld **Unternehmen** ein anderes Unternehmen aus.
4. Wählen Sie das Symbol ![Glühbirne, die die Tell Me Funktion öffnet](media/ui-search/search_small.png "Tell Me-Funktion"), geben Sie **Unternehmen** ein und wählen Sie dann den entsprechenden Link.  
5. Auf der Seite **Unternehmen** wählen Sie **Liste bearbeiten** aus.  
6. Ändern den Namen des Postens *Mein Unternehmen* in etwas anderes.  

    Warten Sie mehrere Minuten. Wir machen einige Änderungen in der zugrunde liegenden Datenbank und das kann eine Weile dauern.
7.  Wenn die Anwendung wieder bereit steht, wählen Sie die Schaltfläche **Neues Unternehmen erstellen** aus.  
8.  Im Dialogfeld, das erscheint, geben Sie den Namen als *Mein Unternehmen* an, und wählen Sie die Option **Suiten-Produktion – nur Einrichtungsdaten** aus.  

Dies kann wieder mehrere Minuten dauern. Wenn der Vorgang abgeschlossen ist, sind Sie in der Lage, auf Invoicing als Teil Ihrer Microsoft 365 Business Standard-Umgebung zuzugreifen. Dies gilt jedoch nur für das Exportieren von Daten, da die Invoicing-App veraltet ist.  

### <a name="what-about-my-data"></a>Informationen zu Ihren Daten.
Wenn Sie die Vorlage Meine Mandanten umbenennen auswählen, werden die Datenbanktabellen, die Ihre bestehenden [!INCLUDE[prod_short](includes/prod_short.md)] Daten speichern, umbenennte, aber die Daten selber werden nicht berührt  

Wenn Sie "Invoicing" und [!INCLUDE[prod_short](includes/prod_short.md)] verwenden, werden die Daten in zwei verschiedenen Containern gespeichert (die zwei Unternehmen). Nichts wird freigegebent, daher müssen Sie Debitoren und Artikel in beiden Unternehmen verwalten.  

## <a name="see-also"></a>Siehe auch
[Häufig gestellte Fragen](across-faq.md)  
[Verwaltung](admin-setup-and-administration.md)  


[!INCLUDE[footer-include](includes/footer-banner.md)]