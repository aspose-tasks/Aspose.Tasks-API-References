---
title: "Tsk.WBS"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Tsk field. 작업 분류 구조 WBS 코드"
type: docs
weight: 1130
url: /ko/net/aspose.tasks/tsk/wbs/
---
## Tsk.WBS field

작업 분류 구조(WBS) 코드.

```csharp
public static readonly Key<string, TaskKey> WBS;
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


