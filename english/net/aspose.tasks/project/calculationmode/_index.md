---
title: Project.CalculationMode
second_title: Aspose.Tasks for .NET API Reference
description: Project property. Gets or sets calculation mode of a project. Can be one of the values of CalculationMode enumeration
type: docs
weight: 110
url: /net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

Gets or sets calculation mode of a project. Can be one of the values of `CalculationMode` enumeration.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## Examples

Shows how to use project calculation mode.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// Set project start date and add new tasks
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// The necessary properties are set in manual mode
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// When we link two tasks together their dates are not recalculated in manual mode
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Task 2 Start has not been changed
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### See Also

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


