---
title: "Project.CalculationMode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Project-eigenschap. Haalt de berekeningsmodus van een project op of stelt deze in. Kan een van de waarden van de CalculationMode-enumeratie zijn"
type: docs
weight: 110
url: /nl/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Haalt de berekeningsmodus van een project op of stelt deze in. Kan een van de waarden van de `CalculationMode`-enumeratie zijn.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Voorbeelden

Toont hoe de projectberekeningsmodus te gebruiken.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Stel de projectbegindatum in en voeg nieuwe taken toe
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// De noodzakelijke eigenschappen zijn ingesteld in de handmatige modus
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// Wanneer we twee taken aan elkaar koppelen, worden hun datums niet opnieuw berekend in de handmatige modus
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Start van Taak 2 is niet gewijzigd
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### Zie ook

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


