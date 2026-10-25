---
title: "Tsk.Resume"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 남은 부분이 진행 상황을 입력한 후 재개될 예정인 날짜입니다."
type: docs
weight: 1000
url: /ko/net/aspose.tasks/tsk/resume/
---
## Tsk.Resume field

작업의 남은 부분이 진행을 시작한 후 재개될 예정인 날짜.

```csharp
public static readonly Key<DateTime, TaskKey> Resume;
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


