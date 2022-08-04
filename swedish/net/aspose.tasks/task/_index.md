---
title: Task
second_title: Aspose.Tasks för .NET API-referens
description: Representerar en uppgift i ett projekt.
type: docs
weight: 2060
url: /sv/net/aspose.tasks/task/
---
## Task class

Representerar en uppgift i ett projekt.

```csharp
public class Task : IEquatable<Task>
```

## Egenskaper

| namn | Beskrivning |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | Hämtar en samling resurstilldelningar för detta objekt. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | Hämtar eller ställer in samlingen av baslinjevärden för uppgiften. |
| [Children](../../aspose.tasks/task/children) { get; } | Hämtar en underordnad uppgiftssamling av detta objekt. TaskCollection-objekt som representerar underordnade uppgifter. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | Hämtar ExtendedAttributeCollection-objekt som innehåller värdena för ett utökat attribut. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | Hämtar eller sätter[`OutlineCodeCollection`](../outlinecodecollection) objekt. |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | Hämtar det överordnade projektet för en uppgift. |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | Hämtar den överordnade uppgiften för en uppgift. |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | Får en[`TaskCollection`](../taskcollection) objekt som innehåller alla föregångare till detta Task-objekt. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | Hämtar instansen av[`RecurringTaskInfo`](../recurringtaskinfo) klass för uppgiften som är en återkommande uppgift; om uppgiften inte är återkommande returneras null;  Informationen för t.ex[`RecurringTaskInfo`](../recurringtaskinfo) finns endast i mpp-filformat. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | Får en SplitPart-samling som representerar delarna av en uppgift. |
| [Successors](../../aspose.tasks/task/successors) { get; } | Får en[`TaskCollection`](../taskcollection) objekt som innehåller alla efterföljare till detta Task-objekt. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | Hämtar eller ställer in ett TimephasedDataCollection-objekt för denna uppgift. Det tidsfasade datablocket associerat med en uppgift. |

## Metoder

| namn | Beskrivning |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | Skapar en fullständig kopia av en uppgift utan deluppgifter. |
| [Delete](../../aspose.tasks/task/delete)() | Tar bort en uppgift från samlingen av överordnade projektuppgifter och alla dess tilldelningar. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | Returnerar ett värde som anger om denna instans är lika med ett angivet objekt. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | Returnerar ett värde som anger om denna instans är lika med en angiven uppgift. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | Returnerar värdet som egenskapen är mappad till i den här behållaren. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | Returnerar ett hashkodvärde för denna uppgift. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | Returnerar[`TimephasedDataCollection`](../timephaseddatacollection) objekt med[`TimephasedData`](./timephaseddata) värden inom givna start- och slutdatum. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | Returnerar[`TimephasedDataCollection`](../timephaseddatacollection) objekt med[`TimephasedData`](./timephaseddata) värden inom givna start- och slutdatum för angiven tidsfasad datatyp. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | Flyttar den aktuella uppgiften till samma dispositionsnivå före en uppgift med det angivna Id. If ParentProject.CalculationMode is None bör användaren anropa Project.Recalculate() efter att ha använt den här metoden (Det kommer att omplanera alla projektuppgifter (start-/slutdatum, sätter tidiga/sena datum) och beräkna de beroende fälten som slacks, work and cost fields, disposition levels). Om ParentProject.CalculationMode är manuell kommer metoden endast att beräkna uppgifts-id, dispositionsnivå och dispositionsnummer automatiskt. If ParentProject. CalculationMode är Automatisk metoden schemalägger alla projekts uppgifter automatiskt (start-/slutdatum, anger tidiga/sena datum, beräknar slacks, arbets- och kostnadsfält, räknar om id och dispositionsnivåer). |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | Flyttar den aktuella uppgiften till samma dispositionsnivå före den angivna uppgiften. Om ParentProject.CalculationMode är Ingen ska användaren anropa Project.Recalculate() efter att ha använt denna metod (Det kommer att omschemalägga alla projektuppgifter (start-/slutdatum, sätter tidigt/ sena datum) och beräkna de beroende fälten såsom slacks, work and cost fields, disposition levels). Om ParentProject.CalculationMode är manuell kommer metoden endast att beräkna uppgifts-id, dispositionsnivå och dispositionsnummer automatiskt. Om ParentProject.CalculationMode är Automatic metoden schemalägger alla projekts uppgifter automatiskt (start-/slutdatum, sätter tidiga/sena datum, beräknar slack-, arbets- och kostnadsfält, räknar om id och dispositionsnivåer). |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | Indrag en uppgift i dispositionen. |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | Marknadsför en uppgift i dispositionen. |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | Samlar rekursivt alla underordnade uppgifter till denna uppgift. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | Mappar den angivna egenskapen till det angivna värdet i den här behållaren. |
| override [ToString](../../aspose.tasks/task/tostring)() | Returnerar kort strängrepresentation av en uppgift. De exakta detaljerna för representationen är ospecificerade och kan komma att ändras. |

### Anmärkningar

De **Uppgift** representerar en enatoms chuck av arbete.

Man kan använda **Uppgift**att planera ett projekt genom att skapa uppgifter och tilldela lämpliga resurser till dem. Uppgifter i ett projekt är organiserade som en rotad hierarkisk trädstruktur, med en rotuppgift och underträd av underordnade uppgifter.

För att bygga ett träd av uppgifter kan man använda en specialiserad samling[`TaskCollection`](../taskcollection) genom att komma åt[`RootTask`](../project/roottask) egendom t.ex.:

```csharp
Project project = new Project();

// lägg till nya uppgifter
Task task1 = project.RootTask.Children.Add(); // en överordnad uppgift med tomt namn läggs till
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // infogar en uppgift före childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// spara projekt i ett av tillgängliga format
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### Se även

* namnutrymme [Aspose.Tasks](../../aspose.tasks)
* hopsättning [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
