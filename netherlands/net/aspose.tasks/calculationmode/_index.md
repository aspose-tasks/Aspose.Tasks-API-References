---
title: "Enum CalculationMode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.CalculationMode enum. Specificeert de projectberekeningsmodus"
type: docs
weight: 210
url: /nl/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

Specificeert de projectberekeningsmodus.

```csharp
public enum CalculationMode
```

### Waarden

| Naam | Waarde | Beschrijving |
| --- | --- | --- |
| None | `0` | Geen. Projectdatums en -kosten worden in deze modus niet opnieuw berekend. |
| Automatic | `1` | Automatische modus. Projectdatums en -kosten worden opnieuw berekend bij gebruik van deze modus. |
| Manual | `2` | Handmatige modus. Alleen noodzakelijke velden worden in deze modus opnieuw berekend, bijvoorbeeld UIDs en ID's van objecten. |

## Voorbeelden

Toont hoe de automatische berekeningsmodus te gebruiken.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// Stel de projectbegindatum in en voeg nieuwe taken toe
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// Taken koppelen
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Controleer of datums opnieuw zijn berekend
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

Toont hoe de geen-berekeningsmodus te gebruiken.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// Voeg een nieuwe taak toe
var task = project.RootTask.Children.Add("Task");

// Let op dat zelfs ID's niet werden berekend            
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// Stel de duur-eigenschap in
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Toont hoe de handmatige berekeningsmodus te gebruiken.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


