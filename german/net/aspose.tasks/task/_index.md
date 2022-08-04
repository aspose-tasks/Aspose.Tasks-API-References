---
title: Task
second_title: Aspose.Tasks für .NET-API-Referenz
description: Stellt eine Aufgabe in einem Projekt dar.
type: docs
weight: 2060
url: /de/net/aspose.tasks/task/
---
## Task class

Stellt eine Aufgabe in einem Projekt dar.

```csharp
public class Task : IEquatable<Task>
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Ruft eine Sammlung von Ressourcenzuweisungen für dieses Objekt ab. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Ruft die Sammlung von Baseline-Werten der Aufgabe ab oder legt sie fest. |
| [Children](../../aspose.tasks/task/children) { get; } | Ruft eine untergeordnete Aufgabensammlung dieses Objekts ab. TaskCollection-Objekt, das untergeordnete Aufgaben darstellt. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Ruft das ExtendedAttributeCollection-Objekt ab, das die Werte eines erweiterten Attributs enthält. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Holt oder setzt[`OutlineCodeCollection`](../outlinecodecollection) Objekt. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Ruft das übergeordnete Projekt einer Aufgabe ab. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Ruft die übergeordnete Aufgabe einer Aufgabe ab. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | erhält a[`TaskCollection`](../taskcollection) Objekt, das alle Vorgänger dieses Task-Objekts enthält. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Ruft die Instanz von ab[`RecurringTaskInfo`](../recurringtaskinfo) Klasse für die Aufgabe, die eine wiederkehrende Aufgabe ist; wenn die Aufgabe nicht wiederkehrend ist, wird null zurückgegeben;  Die Informationen für die Instanz von[`RecurringTaskInfo`](../recurringtaskinfo) liegt nur im mpp-Dateiformat vor. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Ruft eine SplitPart-Sammlung ab, die die Teile einer Aufgabe darstellt. |
| [Successors](../../aspose.tasks/task/successors) { get; } | erhält a[`TaskCollection`](../taskcollection) Objekt, das alle Nachfolger dieses Task-Objekts enthält. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Ruft ein TimephasedDataCollection-Objekt dieser Aufgabe ab oder legt es fest. Der mit einer Aufgabe verknüpfte Zeitphasen-Datenblock. |

## Methoden

| Name | Beschreibung |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Erstellt eine vollständige Kopie einer Aufgabe ohne Unteraufgaben. |
| [Delete](../../aspose.tasks/task/delete)() | Löscht eine Aufgabe aus der Aufgabensammlung des übergeordneten Projekts und alle ihre Zuweisungen. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Gibt einen Wert zurück, der angibt, ob diese Instanz gleich einem angegebenen Objekt ist. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Gibt einen Wert zurück, der angibt, ob diese Instanz gleich einer angegebenen Aufgabe ist. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Gibt den Wert zurück, dem die Eigenschaft in diesem Container zugeordnet ist. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Gibt einen Hash-Code-Wert für diese Aufgabe zurück. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | gibt zurück[`TimephasedDataCollection`](../timephaseddatacollection) Objekt mit[`TimephasedData`](./timephaseddata) Werte innerhalb des angegebenen Start- und Enddatums. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | gibt zurück[`TimephasedDataCollection`](../timephaseddatacollection) Objekt mit[`TimephasedData`](./timephaseddata) Werte innerhalb der angegebenen Start- und Enddaten des angegebenen Zeitphasen-Datentyps. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Verschiebt die aktuelle Aufgabe auf derselben Gliederungsebene vor eine Aufgabe mit der angegebenen ID. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer Project.Recalculate() aufrufen, nachdem er diese Methode verwendet hat (Es wird alle Projektaufgaben neu planen (Start-/Enddaten, legt frühe/späte Termine fest) und berechnet die abhängigen Felder wie Lücken, Arbeits- und Kostenfelder, Gliederungsebenen). Wenn ParentProject.CalculationMode Manuell ist, berechnet die Methode nur Aufgaben-ID, Gliederungsebene und Gliederungsnummern automatisch. Wenn ParentProject. CalculationMode ist Automatic, die Methode plant alle Projektaufgaben automatisch neu (Start-/Endtermine, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder, berechnet IDs und Gliederungsebenen neu). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Verschiebt die aktuelle Aufgabe auf derselben Gliederungsebene vor die angegebene Aufgabe. Wenn ParentProject.CalculationMode None ist, sollte der Benutzer Project.Recalculate() aufrufen, nachdem er diese Methode verwendet hat späte Termine) und berechnen Sie die abhängigen Felder wie Lücken, Arbeits- und Kostenfelder, Gliederungsebenen). Wenn ParentProject.CalculationMode Manuell ist, berechnet die Methode nur Aufgaben-ID, Gliederungsebene und Gliederungsnummern automatisch. Wenn ParentProject.CalculationMode Automatisch ist Die Methode plant alle Projektaufgaben automatisch neu (Start-/Endtermine, legt frühe/späte Termine fest, berechnet Lücken, Arbeits- und Kostenfelder, berechnet IDs und Gliederungsebenen neu). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Rückt eine Aufgabe in die Gliederung ein. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Fördert eine Aufgabe in der Gliederung. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Sammelt rekursiv alle untergeordneten Aufgaben dieser Aufgabe. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Ordnet die angegebene Eigenschaft dem angegebenen Wert in diesem Container zu. |
| override [ToString](../../aspose.tasks/task/tostring)() | Gibt eine kurze Zeichenfolgendarstellung einer Aufgabe zurück. Die genauen Details der Darstellung sind nicht spezifiziert und können sich ändern. |

### Bemerkungen

Das **Aufgabe** repräsentiert ein atomares Chuck an Arbeit.

Kann man verwenden **Aufgabe**um ein Projekt zu planen, indem Aufgaben erstellt und ihnen entsprechende Ressourcen zugewiesen werden. Aufgaben in einem Projekt sind als verwurzelte hierarchische Baumstruktur organisiert, mit einer Stammaufgabe und Unterbäumen von untergeordneten Aufgaben.

Um einen Aufgabenbaum zu erstellen, kann man eine spezialisierte Sammlung verwenden[`TaskCollection`](../taskcollection) durch Zugriff[`RootTask`](../project/roottask) Eigentum zB:

```csharp
Project project = new Project();

// neue Aufgaben hinzufügen
Task task1 = project.RootTask.Children.Add(); // eine übergeordnete Aufgabe mit leerem Namen wird hinzugefügt
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // fügt eine Aufgabe vor der childTask3 ein
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// Projekt in einem der verfügbaren Formate speichern
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Siehe auch

* namensraum [Aspose.Tasks](../../aspose.tasks)
* Montage [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
