---
title: "TaskCollection.Add"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "TaskCollection methode. Voeg de opgegeven taak toe aan de instantie van de TaskCollection-klasse. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate aanroepen na het gebruik van deze methode. Het zal alle projecttaken opnieuw plannen: start/einddatums, stelt vroege/late datums in en berekent de afhankelijke velden zoals speling, werk en kostengegevens, id's en outline-niveaus. Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak-id, outline-niveau en outline-nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle projecttaken automatisch opnieuw: start/einddatums, stelt vroege/late datums in, berekent speling, werk en kostengegevens, en herberekent id's en outline-niveaus."
type: docs
weight: 50
url: /nl/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

Voeg de opgegeven taak toe aan de instantie van de [`TaskCollection`](../) klasse. Als ParentProject.CalculationMode None is, moet de gebruiker Project.Recalculate() aanroepen na het gebruik van deze methode (het zal alle projecttaken opnieuw plannen (start/einddatums, stelt vroege/late datums in) en de afhankelijke velden berekenen zoals speling, werk en kostengegevens, id's en outline-niveaus). Als ParentProject.CalculationMode Manual is, berekent de methode alleen taak-id, outline-niveau en outline-nummers automatisch. Als ParentProject.CalculationMode Automatic is, plant de methode alle taken van het project automatisch opnieuw (start/einddatums, stelt vroege/late datums in, berekent speling, werk en kostengegevens, herberekent id's en outline-niveaus).

```csharp
public void Add(Task item)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| item | Taak | de opgegeven taak die aan deze taakverzameling moet worden toegevoegd. |

## Voorbeelden

Toont hoe een taak onder een andere ouder kan worden verplaatst.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Taken ophalen op Id's
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Taak 6 toevoegen aan een andere ouder
task2.Children.Add(task);
```

### Zie ook

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Voegt een nieuwe taak toe aan de projecttakenverzameling op hetzelfde outline-niveau als de laatste taak.

```csharp
public Task Add()
```

### Retourwaarde

geeft de nieuw toegevoegde instantie van de [`Task`](../../task/) klasse terug.

## Voorbeelden

Toont hoe te werken met taakcollecties.

```csharp
var project = new Project();

// de taakcollectie is niet alleen-lezen en kan worden uitgebreid
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// taken maken
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// projecttaken afdrukken
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// een taak kan uit de collectie worden gehaald op basis van ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// of op basis van UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// ook kan men een terugkerende taak toevoegen
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// de eerste taak in een reeks wordt geretourneerd
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// de collectie kan worden geconverteerd naar een eenvoudige lijst
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Zie ook

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Voegt een nieuwe taak toe aan de verzameling van onderliggende taken.

```csharp
public Task Add(string taskName)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskName | String | de opgegeven taaknaam. |

### Retourwaarde

geeft de nieuw toegevoegde instantie van de [`Task`](../../task/) klasse terug.

## Voorbeelden

Toont hoe te werken met taakcollecties.

```csharp
var project = new Project();

// de taakcollectie is niet alleen-lezen en kan worden uitgebreid
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// taken maken
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// projecttaken afdrukken
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// een taak kan uit de collectie worden gehaald op basis van ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// of op basis van UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// ook kan men een terugkerende taak toevoegen
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// de eerste taak in een reeks wordt geretourneerd
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// de collectie kan worden geconverteerd naar een eenvoudige lijst
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Zie ook

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Voegt een nieuwe terugkerende taak toe aan de verzameling van onderliggende taken.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| taskName | String | de opgegeven taaknaam. |
| beforeTaskId | Int32 | De opgegeven id van een taak vóór welke een nieuwe taak wordt ingevoegd. |

### Retourwaarde

geeft een taak terug die vóór een taak met de opgegeven id is ingevoegd.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException wordt gegooid als de opgegeven id geen geldige taak-id is. |

## Voorbeelden

Toont hoe te werken met taakcollecties.

```csharp
var project = new Project();

// de taakcollectie is niet alleen-lezen en kan worden uitgebreid
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// taken maken
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// projecttaken afdrukken
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// een taak kan uit de collectie worden gehaald op basis van ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// of op basis van UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// ook kan men een terugkerende taak toevoegen
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// de eerste taak in een reeks wordt geretourneerd
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// de collectie kan worden geconverteerd naar een eenvoudige lijst
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Zie ook

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Voegt een nieuwe taak in vóór een taak met de opgegeven id en op hetzelfde outline-niveau.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parameter | Type | Beschrijving |
| --- | --- | --- |
| parameters | RecurringTaskParameters | De parameters die zijn opgegeven voor het aanmaken van een terugkerende taak. |

### Retourwaarde

geeft de nieuw toegevoegde instantie van de [`Task`](../../task/) klasse terug.

### Uitzonderingen

| exceptie | conditie |
| --- | --- |
| ArgumentNullException | Wordt gegooid als de opgegeven parameters null zijn. |
| ArgumentException | Wordt gegooid als de opgegeven parameters ongeldig zijn. |

## Voorbeelden

Toont hoe te werken met taakcollecties.

```csharp
var project = new Project();

// de taakcollectie is niet alleen-lezen en kan worden uitgebreid
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// taken maken
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// projecttaken afdrukken
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// een taak kan uit de collectie worden gehaald op basis van ID
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// of op basis van UID
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// ook kan men een terugkerende taak toevoegen
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// de eerste taak in een reeks wordt geretourneerd
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// de collectie kan worden geconverteerd naar een eenvoudige lijst
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Zie ook

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


