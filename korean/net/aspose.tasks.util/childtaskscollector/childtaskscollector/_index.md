---
title: "ChildTasksCollector.ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ChildTasksCollector 생성자. ChildTasksCollector 클래스의 새 인스턴스를 초기화합니다."
type: docs
weight: 10
url: /ko/net/aspose.tasks.util/childtaskscollector/childtaskscollector/
---
## ChildTasksCollector constructor

[`ChildTasksCollector`](../) 클래스의 새 인스턴스를 초기화합니다.

```csharp
public ChildTasksCollector()
```

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

* class [ChildTasksCollector](../)
* namespace [Aspose.Tasks.Util](../../childtaskscollector/)
* assembly [Aspose.Tasks](../../../)


