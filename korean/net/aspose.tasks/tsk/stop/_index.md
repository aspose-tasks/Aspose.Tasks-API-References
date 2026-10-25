---
title: "Tsk.Stop"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 실제 부분이 끝나는 날짜를 나타냅니다."
type: docs
weight: 1060
url: /ko/net/aspose.tasks/tsk/stop/
---
## Tsk.Stop field

작업 실제 부분의 종료를 나타내는 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> Stop;
```

## 예제

작업의 Stop/Resume 날짜를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "StopResumeDates.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 모든 작업의 Stop 및 Resume 날짜를 확인합니다.
foreach (var task in collector.Tasks)
{
    if (task.Get(Tsk.Stop).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Stop: NA");
    }
    else
    {
        Console.WriteLine("Stop: " + task.Get(Tsk.Stop).ToShortDateString());
    }

    if (task.Get(Tsk.Resume).ToShortDateString() == "1/1/2000")
    {
        Console.WriteLine("Resume: NA");
    }
    else
    {
        Console.WriteLine("Resume: " + task.Get(Tsk.Resume).ToShortDateString());
    }
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


