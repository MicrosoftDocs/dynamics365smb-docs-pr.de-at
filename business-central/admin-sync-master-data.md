---
title: Masterdatensynchronisierung verwalten
description: Erfahren wie Sie die Masterdatensynchronisierung verwalten.
author: brentholtorf
ms.author: bholtorf
ms.reviewer: bholtorf
ms.service: dynamics-365-business-central
ms.topic: conceptual
ms.date: 04/05/2024
ms.custom: bap-template
ms.search.form: '7230, 7233, 5338, 7236, 672, 7234'
---
# <a name="manage-master-data-synchronization"></a>Masterdatensynchronisierung verwalten

Nachdem Sie die Stammdatensynchronisierung eingerichtet und zum ersten Mal synchronisiert haben, werden Datensätze in den ausgewählten Tabellen gekoppelt und für jede Tabelle wird ein wiederkehrender Auftragswarteschlangeneintrag erstellt. Die Aufgabenverwlaltungseinträge synchronisieren automatisch Daten in den Tochterunternehmen, wenn jemand eine Änderung im Quellunternehmen vornimmt. Ansonsten brauchen Sie nichts zu tun.

> [!NOTE]
> Standardmäßig werden die Aufgabenwarteschlangeneinträge jede Minute ausgeführt, und Sie können den Zeitplan nicht ändern.

Manchmal gehen jedoch Dinge schief, und es kann Situationen geben, die Sie verwalten oder untersuchen müssen. Wenn beispielsweise Personen denselben Datensatz sowohl im Quellunternehmen als auch in einer Tochtergesellschaft ändern, schlägt die Synchronisierung fehl, sodass Sie die richtige Änderung angeben können. Oder das Quellunternehmen installiert möglicherweise eine Erweiterung, die das Schema einer der Tabellen ändert, die Sie synchronisieren, indem es ein oder zwei Felder hinzufügt. Wenn Sie die neuen Felder in den Tochterunternehmen synchronisieren möchten, müssen Sie dieselben Erweiterungen installieren und die Tabellenschemata in deren Einrichtung aktualisieren.

Dieser Artikel beschreibt die Tools, die Sie verwenden können, um eine reibungslose Synchronisierung zu gewährleisten.

## <a name="overwrite-local-changes"></a>Lokale Änderungen überschreiben

Sie können das Kontrollkästchen **Lokale Änderungen überschreiben** für die Felder und Tabellen verwenden, die Sie synchronisieren, um zuzulassen, dass Daten aus dem Quellunternehmen Daten im Tochterunternehmen überschreiben.

> [!NOTE]
> Sie können die Synchronisierung eines Felds nicht aktivieren und der Tochtergesellschaft erlauben, unabhängig vom Quellunternehmen Werte darin einzutragen. Sie müssen entweder die Synchronisierung für das Feld deaktivieren oder dem Quellunternehmen erlauben, lokale Änderungen zu überschreiben.

## <a name="update-table-schemas"></a>Tabellenschemata aktualisieren

Wenn das Quellunternehmen eine Tabelle ändert, indem es beispielsweise ein Feld hinzufügt, das Sie synchronisieren möchten, müssen Tochtergesellschaften ihre Feldzuordnungen aktualisieren. Verwenden Sie auf der Seite **Synchronisierungsfelder** die Aktion **Felder aktualisieren**.

## <a name="enable-or-disable-couplings-between-records"></a>Aktivieren oder deaktivieren Sie Kopplungen zwischen Datensätzen

Um die Kopplung für bestimmte Datensätze in einer Tabelle zu starten oder zu beenden, wählen Sie auf der Seite **Synchronisationsfelder** die Felder aus und verwenden Sie dann entweder die **Aktivieren** oder **Aktionen deaktivieren**.

> [!TIP]
> Eine schnelle Möglichkeit, mehrere Felder gleichzeitig zu aktivieren oder zu deaktivieren, besteht darin, sie in der Liste auszuwählen und dann die Aktionen **Aktivieren** oder **Deaktivieren** zu verwenden.

## <a name="run-a-full-synchronization"></a>Ausführen einer vollständigen Synchronisierung

Die Aktion **Vollständige Synchronisierung ausführen** plant eine Synchronisierung für alle Tabellendatensätze im Quellunternehmen und synchronisiert alle Datensätze bedingungslos erneut. Beispielsweise ist eine erneute Synchronisierung nützlich, wenn Sie ein zusätzliches Feld in einer Synchronisierungstabelle aktivieren oder mithilfe der Aktion **Felder aktualisieren** ein zusätzliches Feld hinzufügen. Die Aktion synchronisiert die Daten in diesen Feldern nachträglich.

## <a name="synchronize-modified-records"></a>Bearbeitete Datensätze synchronisieren

Wenn Sie eine Einstellung für eine Tabelle oder ein Feld in einer Tochtergesellschaft ändern, müssen Sie die Synchronisation aktualisieren. Um die Synchronisierung zu aktualisieren, verwenden Sie die Aktion **Geänderte Datensätze synchronisieren** auf der Seite **Synchronisierungstabellen** .

Die Aktion **Geänderte Datensätze synchronisieren** plant eine Synchronisierung der folgenden Tabellendatensätze:

* Datensätze, deren Synchronisierung beim letzten Versuch fehlgeschlagen ist.
* Datensätze, die im Quellunternehmen nach der letzten geplanten Synchronisierung geändert wurden. Sie können den letzten geplanten Synchronisierungszeitpunkt auf der Seite **Synchronisierungstabellen** im Feld **Änderungen synchronisieren seit** überprüfen.

Die Aktion funktioniert genauso wie eine geplante Synchronisierung und Sie können sie verwenden, um außerhalb des Zeitplans zu synchronisieren. Wenn Sie beispielsweise das Kontrollkästchen **Lokale Änderung überschreiben** in einem Feld aktivieren, damit Daten aus dem Quellunternehmen lokale Änderungen überschreiben können, aktualisiert die Aktion diese Daten. Sie können auch einfach warten, bis die nächste geplante Synchronisierung erfolgt.

## <a name="investigate-the-status-of-synchronization"></a>Den Status von Synchronisationsaufträgen anzeigen

Auf der Seite **Synchronisierungstabellen** gibt es zwei Aktionen, mit denen Sie Ihre Synchronisierung überwachen können:

* **Integrationssynchronisierungsaufträge**
* **Aufgabenwarteschlangenposten**

Die Optionen werden in den folgenden Aktionen beschrieben.

|Seite  |Description  |
|---------|---------|
|**Integrationssynchronisierungsaufträge**     | Öffnen Sie die Seite **Auftrags-Integrationssynchronisierung**, um zu untersuchen, was jedes Mal geschah, wenn ein Aufgabenwarteschlangeneintrag ausgeführt wurde. Wählen Sie die Zahlen in den Spalten **Eingefügt** oder **Fehlgeschlagen** aus, um mehr über die Details zu neu hinzugefügten Datensätzen zu erfahren oder herauszufinden, warum ein Datensatz nicht synchronisiert werden konnte. Sie können diese Seite auch verwenden, um ältere Datensätze zu bereinigen, die Sie möglicherweise nicht benötigen. Weitere Informationen zum Bereinigen finden Sie unter [Alte Einträge bereinigen](#clean-up-old-entries).        |
|**Aufgabenwarteschlangenposten**     | Greifen Sie auf Details über den Aufgabenwarteschlangeneintrag zu, der Daten für eine ausgewählte Tabelle synchronisiert. Verwenden Sie diese Seite beispielsweise, um den Status des Auftragswarteschlangeneintrags zu verwalten. Weitere Informationen zu Auftragswarteschlangeneinträgen finden Sie unter [Auftragswarteschlangen zum Planen von Aufgaben verwenden](admin-job-queues-schedule-tasks.md).     |

> [!NOTE]
> Wenn Sie auf der Seite **Integrationssynchronisierung von Aufgaben** einen Fehler finden, den Sie nicht selbst beheben können, ist es hilfreich, die Fehlermeldung anzugeben, wenn Sie sich an Ihren Partner oder an Microsoft wenden, um Support und Callstack-Informationen zu erhalten.

## <a name="clean-up-old-entries"></a>Bereinigen Sie alte Einträge

Im Laufe der Zeit wird die Anzahl der Einträge im Synchronisationsprotokoll groß, sodass Sie möglicherweise ein wenig Ordnung schaffen sollten, um unnötige Einträge zu entfernen. Um das Bereinigen alter Einträge zu vereinfachen, bietet die Seite **Auftrags-Integrationsynchronisierung** die folgenden Aktionen:

* **Posten löschen, die über 7 Tage alt sind**
* **Alle Einträge löschen**

## <a name="adding-extensions"></a>Erweiterungen hinzufügen

Wenn das Quellunternehmen eine neue Erweiterung installiert, muss die Tochtergesellschaft diese ebenfalls installieren, wenn sie Daten dafür synchronisieren möchte. Die Tochtergesellschaft kann die Aktion **Felder aktualisieren** auf der Seite **Synchronisierungsfelder** verwenden, um die Tabellen aus der Erweiterung zu hinzuzufügen Liste.

> [!NOTE]
> Einige Tabellen erhalten Daten aus verknüpften Tabellen. Wenn Sie eine Erweiterung hinzufügen, die keine verknüpften Tabellen enthält, sind die Felder in diesen Tabellen nicht verfügbar. Vergewissern Sie sich, dass Sie alle verknüpften Tabellen hinzugefügt haben.

<!--
## <a name="recreate-a-deleted-job-queue-entry"></a>Recreate a deleted job queue entry

If the recurring job queue entry is deleted for a table, you can quickly recreate it. On the **Synchronization Tables** page, choose the **Use Default Synchronization Setup** action.
-->

## <a name="see-also"></a>Siehe auch

[Vorbereitung der Synchronisierung der Masterdaten](admin-set-up-data-sync.md)
