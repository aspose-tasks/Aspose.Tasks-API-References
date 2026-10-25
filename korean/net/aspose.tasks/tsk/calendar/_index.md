---
title: "Tsk.Calendar"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업 캘린더"
type: docs
weight: 160
url: /ko/net/aspose.tasks/tsk/calendar/
---
## Tsk.Calendar field

작업 캘린더.

```csharp
public static readonly Key<Calendar, TaskKey> Calendar;
```

## 예제

작업 캘린더를 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ReadTaskCalendar.mpp");
var task = project.RootTask.Children.Add("Task1");

// 캘린더를 생성하고 작업에 할당합니다.
var newCalendar = project.Calendars.Add("TaskCal1");
task.Set(Tsk.Calendar, newCalendar);

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 재귀적인 모든 하위 항목을 파싱합니다.
foreach (var tsk in collector.Tasks)
{
    var calendar = tsk.Get(Tsk.Calendar);
    Console.WriteLine("Task calendar name: {0}", calendar == null ? "None" : calendar.Name);
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Calendar](../../calendar/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


