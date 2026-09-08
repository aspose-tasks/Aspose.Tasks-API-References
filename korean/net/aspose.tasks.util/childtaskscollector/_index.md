---
title: "클래스 ChildTasksCollector"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.ChildTasksCollector 클래스. 모든 하위 작업을 수집합니다."
type: docs
weight: 2690
url: /ko/net/aspose.tasks.util/childtaskscollector/
---
## ChildTasksCollector class

모든 하위 작업을 수집합니다.

```csharp
public class ChildTasksCollector : TreeAlgorithmBase<Task>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [ChildTasksCollector](childtaskscollector/)() | `ChildTasksCollector` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [Tasks](../../aspose.tasks.util/childtaskscollector/tasks/) { get; } | 수집된 하위 객체(작업) 목록을 가져옵니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| override [Alg](../../aspose.tasks.util/childtaskscollector/alg/)(Task, int) | 지정된 객체를 처리합니다. |
| virtual [PostAlg](../../aspose.tasks.util/treealgorithmbase-1/postalg/)(Task, int) |  |
| virtual [PreAlg](../../aspose.tasks.util/treealgorithmbase-1/prealg/)(Task, int) |  |

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

* class [TreeAlgorithmBase&lt;T&gt;](../treealgorithmbase-1/)
* class [Task](../../aspose.tasks/task/)
* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


