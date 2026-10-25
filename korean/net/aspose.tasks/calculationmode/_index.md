---
title: "열거형 CalculationMode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.CalculationMode 열거형. 프로젝트 계산 모드를 지정합니다."
type: docs
weight: 210
url: /ko/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

프로젝트 계산 모드를 지정합니다.

```csharp
public enum CalculationMode
```

### 값들

| 이름 | 값 | 설명 |
| --- | --- | --- |
| None | `0` | None. 이 모드에서는 프로젝트 날짜와 비용이 재계산되지 않습니다. |
| Automatic | `1` | Automatic mode. 이 모드를 사용할 때 프로젝트 날짜와 비용이 재계산됩니다. |
| Manual | `2` | Manual mode. 이 모드에서는 필요한 필드만 재계산되며, 예를 들어 객체의 UID와 ID가 포함됩니다. |

## 예제

자동 계산 모드 사용 방법을 보여줍니다.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// 프로젝트 시작 날짜를 설정하고 새 작업을 추가합니다.
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// 작업 연결
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// 날짜가 재계산되었는지 확인합니다.
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

none 계산 모드 사용 방법을 보여줍니다.

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// 새 작업을 추가합니다.
var task = project.RootTask.Children.Add("Task");

// ID조차도 계산되지 않았음을 참고하십시오.
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// duration 속성을 설정합니다.
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

manual 계산 모드 사용 방법을 보여줍니다.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


