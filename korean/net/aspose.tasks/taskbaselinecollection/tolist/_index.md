---
title: "TaskBaselineCollection.ToList"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaselineCollection 메서드. TaskBaselineCollection 객체를 TaskBaseline 객체 목록으로 변환합니다."
type: docs
weight: 60
url: /ko/net/aspose.tasks/taskbaselinecollection/tolist/
---
## TaskBaselineCollection.ToList method

TaskBaselineCollection 객체를 [`TaskBaseline`](../../taskbaseline/) 객체 목록으로 변환합니다.

```csharp
public List<TaskBaseline> ToList()
```

### 반환 값

[`TaskBaseline`](../../taskbaseline/) 객체 목록.

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

* class [TaskBaseline](../../taskbaseline/)
* class [TaskBaselineCollection](../)
* namespace [Aspose.Tasks](../../taskbaselinecollection/)
* assembly [Aspose.Tasks](../../../)


