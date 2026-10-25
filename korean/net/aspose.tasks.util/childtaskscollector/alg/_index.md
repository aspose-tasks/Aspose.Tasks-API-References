---
title: "ChildTasksCollector.Alg"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ChildTasksCollector 메서드. 지정된 객체를 처리합니다."
type: docs
weight: 30
url: /ko/net/aspose.tasks.util/childtaskscollector/alg/
---
## ChildTasksCollector.Alg method

지정된 객체를 처리합니다.

```csharp
public override void Alg(Task el, int level)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| el | 작업 | 처리할 객체. |
| 레벨 | Int32 | 트리 노드 레벨. |

## 예제

프로젝트의 모든 작업을 평범한 목록으로 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "ParentChildTasks.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);

// 수집된 모든 작업을 파싱합니다
foreach (var task in collector.Tasks)
{
    Console.WriteLine(task.Get(Tsk.Name));
}
```

### 또 보기

* class [Task](../../../aspose.tasks/task/)
* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


