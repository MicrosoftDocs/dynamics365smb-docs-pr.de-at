---
title: Zahlungsformen einrichten
description: 'Sie können Zahlungsformen nutzen, z.B. Banküberweisung, Kasse oder PayPal, um festzulegen, wie eine Rechnung bezahlt wird.'
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.topic: conceptual
ms.devlang: al
ms.search.keywords: 'check, bank transfer, cash, PayPal'
ms.search.form: '427,'
ms.date: 06/10/2024
ms.service: dynamics-365-business-central
---
# <a name="set-up-payment-methods"></a>Zahlungsformen einrichten

Zahlungsformen definieren die Art, wie Sie es vorziehen, dass Debitoren Sie zahlen und wie Sie den Kreditoren bezahlen können. Die Methode kann für jeden Debitor oder Kreditor variieren. Beispiele für typische Zahlungsformen sind **Bankkonten**, **Bargeld**, **Check** oder **Konto**.

Sie können eine Zahlungsform Debitoren und Kreditoren zuweisen, sodass dasselbe Verfahren  immer auf Verkaufs- und Einkaufsbelegen verwendet wird, die Sie für sie einrichten. Bei Bedarf können Sie die Methode im Einkaufs- und Verkaufsbeleg ändern. Wenn Sie beispielsweise eine bestimmte Einkaufsrechnung in bar anstatt mit Scheck bezahlen möchten. Die standardmäßige Zahlungsform, die dem Kreditor zugeordnet ist, wird nicht verändert.

Die gleichen Zahlungsformen werden für Einkaufs- und Verkaufsbelegen verwendet. Beispielsweise wird die Zahlungsform _cash_ verwendet, um Zahlungen zu leisten und zu empfangen. [!INCLUDE[prod_short](includes/prod_short.md)] weiß, dass wenn Sie eine Verkaufsrechnung erstellen, Sie eine Zahlung erwarten und das Gegenteil der Einkaufsrechnungen ist.

Gutschriften für Reklamationen sind jedoch Ausnahmen, da Geld entgegengesetzt fließt, von Ihnen an Ihren Kunden und von Ihrem Lieferanten an Sie. Daher wird eine standardmäßige Zahlungsform nicht den Gutschriften zugeordnet. Es gibt jedoch eine Problemumgehung. Sie können Zahlungsbedingungen für den Debitor oder Kreditor festlegen. Auch wenn das Feld **Skonto auf Gutschrift berech.** nicht für diese Problemumgehung beabsichtigt ist, wird bei Aktivierung des Kontrollkästchens auf der Seite **Zahlungsbedingungen** eine standardmäßige Zahlungsform hinzugefügt, wenn Sie eine Gutschrift erstellen. <br><br>  

> [!Video https://www.microsoft.com/videoplayer/embed/RE476Ys?rel=0]

## <a name="to-set-up-a-payment-method"></a>So richten Sie eine Zahlungsform ein

[!INCLUDE[prod_short](includes/prod_short.md)] enthält mehrere Zahlungsformen, die Geschäfte häufig verwenden. Sie können so viele Zeilen hinzufügen, wie Sie benötigen.

1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](media/ui-search/search_small.png "Tell me-Funktion") Symbol. Geben Sie **Zahlungsformen** ein, und wählen Sie dann den entsprechenden Link.
2. Füllen Sie die Felder je nach Bedarf aus. [!INCLUDE[tooltip-inline-tip](includes/tooltip-inline-tip_md.md)]

Fügen Sie Ihren Zahlungsbedingungen optional Ihre Zahlungsform hinzu. Weitere Informationen finden Sie unter [Einrichten von Zahlungbedingungen](finance-payment-terms.md).  

## <a name="to-assign-a-payment-method-to-a-customer-or-vendor"></a>So weisen Sie einem Kreditor eine Zahlungsform zu

1. Wählen Sie die ![Glühbirne, die die „Wie möchten Sie weiter verfahren“-Funktion öffnet.](media/ui-search/search_small.png "Tell me-Funktion") Symbol. Geben Sie **Kunde** oder **Kreditor** ein und wählen Sie dann den zugehörigen Link.
2. Im **Zahlungsformcode** Feld wählen Sie die Methode, die Sie für den Debitor oder Kreditor standardmäßig verwenden möchten.

## <a name="see-also"></a>Siehe auch

[Neue Debitoren registrieren](sales-how-register-new-customers.md)  
[Zahlungsbedingungen einrichten](finance-payment-terms.md)  
[Finanzen](finance.md)  
[Arbeiten mit [!INCLUDE[prod_short](includes/prod_short.md)]](ui-work-product.md)  

[!INCLUDE[footer-include](includes/footer-banner.md)]
