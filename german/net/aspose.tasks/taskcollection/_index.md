---
title: Class TaskCollection
second_title: Aspose.Tasks für .NET-API-Referenz
description: Aspose.Tasks.TaskCollection klas. Repräsentiert eine Sammlung vonTask Objekte.
type: docs
weight: 2100
url: /de/net/aspose.tasks/taskcollection/
---
## TaskCollection class

Repräsentiert eine Sammlung von[`Task`](../task/) Objekte.

```csharp
public class TaskCollection : IList<Task>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | Ruft die Anzahl der in der TaskCollection enthaltenen Objekte ab. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Ruft einen Wert ab, der angibt, ob diese Sammlung schreibgeschützt ist. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Gibt das Element am angegebenen Index zurück. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | Ruft das übergeordnete Projekt des TaskCollection-Objekts ab. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Fügt der Projektaufgabensammlung eine neue Aufgabe auf derselben Gliederungsebene wie die letzte Aufgabe hinzu. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Fügt eine neue Aufgabe vor einer Aufgabe mit der angegebenen ID und auf derselben Gliederungsebene ein. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Fügt der Kinderaufgabensammlung eine neue Aufgabe hinzu. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | Fügen Sie die angegebene Aufgabe der Instanz von hinzu`TaskCollection`class. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer Project.Recalculate() aufrufen, nachdem er diese Methode verwendet hat (es wird alle Projektaufgaben neu planen (Start-/Endtermine, frühe/späte Termine festlegen) und die abhängigen Felder wie Lücken, Arbeit berechnen und Kostenfelder, IDs und Gliederungsebenen). Wenn ParentProject.CalculationMode Manuell ist, berechnet die Methode nur Aufgaben-ID, Gliederungsebene und Gliederungsnummern automatisch. Wenn ParentProject.CalculationMode Automatisch ist, plant die Methode alle Projektaufgaben automatisch neu (Start/Ende Termine, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder, berechnet IDs und Gliederungsebenen neu). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Fügt eine neue wiederkehrende Aufgabe zur Sammlung untergeordneter Aufgaben hinzu. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Überprüft, ob die Sammlung das angegebene Element enthält. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Gibt eine Aufgabe mit der angegebenen ID zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Gibt eine Aufgabe mit der angegebenen Uid zurück, deren Vorgänger die übergeordnete Aufgabe dieser Sammlung ist. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Gibt einen Enumerator für diese Sammlung zurück. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Dies ist die Stub-Implementierung der Insert -Methode von IList, die nur NotSupportedException auslöst. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Dies ist die Stub-Implementierung der Remove -Methode von ICollection, die nur NotSupportedException auslöst. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | Konvertiert das TaskCollection-Objekt in eine Liste von[`Task`](../task/) Objekte. |

### Siehe auch

* class [Task](../task/)
* namensraum [Aspose.Tasks](../../aspose.tasks/)
* Montage [Aspose.Tasks](../../)


