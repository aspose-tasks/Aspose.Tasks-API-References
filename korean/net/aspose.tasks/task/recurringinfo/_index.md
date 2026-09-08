---
title: "Task.RecurringInfo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업이 반복 작업인 경우 해당 작업에 대한 RecurringTaskInfo 클래스 인스턴스를 가져오며, 반복 작업이 아닌 경우 null을 반환합니다. RecurringTaskInfo 인스턴스에 대한 정보는 mpp 파일 형식에만 존재합니다."
type: docs
weight: 1030
url: /ko/net/aspose.tasks/task/recurringinfo/
---
## Task.RecurringInfo property

반복 작업인 경우 작업에 대한 [`RecurringTaskInfo`](../../recurringtaskinfo/) 클래스 인스턴스를 가져오며; 반복 작업이 아닌 경우 null을 반환합니다; [`RecurringTaskInfo`](../../recurringtaskinfo/) 인스턴스에 대한 정보는 mpp 파일 형식에만 존재합니다.

```csharp
public RecurringTaskInfo RecurringInfo { get; }
```

## 예제

작업의 반복 정보를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TestRecurringTask2016.mpp");

var task = project.RootTask.Children.GetById(1);

Console.WriteLine("Recurrence Pattern: " + task.RecurringInfo.RecurrencePattern);
Console.WriteLine("Start Date: " + task.RecurringInfo.StartDate);
Console.WriteLine("End Date: " + task.RecurringInfo.EndDate);
Console.WriteLine("Duration: " + task.RecurringInfo.Duration);
Console.WriteLine("Occurrences: " + task.RecurringInfo.Occurrences);
Console.WriteLine("Weekly Days: " + task.RecurringInfo.WeeklyDays);
Console.WriteLine("WeeklyRepetitions: " + task.RecurringInfo.WeeklyRepetitions);
```

### 또 보기

* class [RecurringTaskInfo](../../recurringtaskinfo/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


