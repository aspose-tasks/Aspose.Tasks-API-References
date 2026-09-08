---
title: "클래스 TaskBaselineCollection"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskBaselineCollection 클래스. TaskBaseline 객체의 컬렉션을 나타냅니다"
type: docs
weight: 2380
url: /ko/net/aspose.tasks/taskbaselinecollection/
---
## TaskBaselineCollection class

[`TaskBaseline`](../taskbaseline/) 객체의 컬렉션을 나타냅니다.

```csharp
public class TaskBaselineCollection : IList<TaskBaseline>
```

## 속성

| 이름 | 설명 |
| --- | --- |
| [Count](../../aspose.tasks/taskbaselinecollection/count/) { get; } | 이 TaskBaselineCollection 객체에 포함된 객체 수를 가져옵니다. |
| [Item](../../aspose.tasks/taskbaselinecollection/item/) { get; set; } | 지정된 인덱스의 요소를 반환합니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [Add](../../aspose.tasks/taskbaselinecollection/add/)(TaskBaseline) | ICollection의 Add 메서드에 대한 스텁 구현으로, NotSupportedException만 발생시킵니다. |
| [GetEnumerator](../../aspose.tasks/taskbaselinecollection/getenumerator/)() | 이 컬렉션에 대한 열거자를 반환합니다. |
| [Remove](../../aspose.tasks/taskbaselinecollection/remove/)(TaskBaseline) | 이 컬렉션에서 기준선을 제거합니다. |
| [ToList](../../aspose.tasks/taskbaselinecollection/tolist/)() | TaskBaselineCollection 객체를 [`TaskBaseline`](../taskbaseline/) 객체 목록으로 변환합니다. |

## 예제

작업 기준선 컬렉션을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project();

// 프로젝트 기준선을 생성합니다
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 작업 기준선을 출력합니다
Console.WriteLine("Count of task baselines: " + task.Baselines.Count);
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration: {0}", baseline.Duration);
    Console.WriteLine("Baseline start: {0}", baseline.Start);
    Console.WriteLine("Baseline finish: {0}", baseline.Finish);
}

// 모든 기준선을 지웁니다
List<TaskBaseline> baselines = task.Baselines.ToList();
for (var i = 0; i < baselines.Count; i++)
{
    task.Baselines.Remove(baselines[i]);
}
```

### 또 보기

* class [TaskBaseline](../taskbaseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


