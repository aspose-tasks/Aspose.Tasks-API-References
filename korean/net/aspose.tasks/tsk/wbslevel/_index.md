---
title: "Tsk.WBSLevel"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk 필드. 작업의 가장 오른쪽 WBS 수준"
type: docs
weight: 1140
url: /ko/net/aspose.tasks/tsk/wbslevel/
---
## Tsk.WBSLevel field

작업의 가장 오른쪽 WBS 레벨.

```csharp
public static readonly Key<string, TaskKey> WBSLevel;
```

## 예제

작업의 WBS 코드를 읽는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "TaskWBS.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.WBS));
    Console.WriteLine(task.Get(Tsk.WBSLevel));
}
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


