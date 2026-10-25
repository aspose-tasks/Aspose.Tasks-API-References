---
title: "Project.CalculationMode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Project 속성. 프로젝트의 계산 모드를 가져오거나 설정합니다. CalculationMode 열거형의 값 중 하나일 수 있습니다"
type: docs
weight: 110
url: /ko/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

프로젝트의 계산 모드를 가져오거나 설정합니다. `CalculationMode` 열거형의 값 중 하나일 수 있습니다.

```csharp
public CalculationMode CalculationMode { get; set; }
```

## 예제

프로젝트 계산 모드를 사용하는 방법을 보여줍니다.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// 프로젝트 시작 날짜를 설정하고 새 작업을 추가합니다.
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// 필요한 속성이 manual 모드에서 설정됩니다.
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// 두 작업을 연결하면 manual 모드에서 날짜가 재계산되지 않습니다.
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// Task 2 시작이 변경되지 않았습니다.
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### 또 보기

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


