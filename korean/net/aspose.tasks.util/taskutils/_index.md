---
title: "클래스 TaskUtils"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Util.TaskUtils 클래스. 작업과 관련된 유용한 작업을 제공하는 도우미 클래스"
type: docs
weight: 2770
url: /ko/net/aspose.tasks.util/taskutils/
---
## TaskUtils class

작업과 관련된 유용한 작업을 제공하는 도우미 클래스.

```csharp
public static class TaskUtils
```

## 메서드

| 이름 | 설명 |
| --- | --- |
| static [Apply](../../aspose.tasks.util/taskutils/apply/)(Task, ITreeAlgorithm&lt;Task&gt;, int) | 지정된 알고리즘을 트리의 각 작업에 적용합니다. |
| static [Filter](../../aspose.tasks.util/taskutils/filter/)(Task, ICondition&lt;Task&gt;) | 조건을 만족하는 작업들의 새로운 트리를 구축합니다. |
| static [Find](../../aspose.tasks.util/taskutils/find/)(Task, ICondition&lt;Task&gt;) | 작업 트리에서 조건을 만족하는 작업을 찾습니다. |
| static [TaskChildrenCount](../../aspose.tasks.util/taskutils/taskchildrencount/)(Task) | 재귀적으로 모든 레벨에서 작업의 하위 작업 수를 계산합니다. |

## 예제

트리 알고리즘을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "Project2.mpp");

// 모든 프로젝트 작업을 수집합니다
var coll = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, coll, 0);

// 작업을 일반 목록처럼 다룹니다
foreach (var task in coll.Tasks)
{
    Console.WriteLine("Task Name: " + task.Get(Tsk.Name));
}
```

### 또 보기

* namespace [Aspose.Tasks.Util](../../aspose.tasks.util/)
* assembly [Aspose.Tasks](../../)


