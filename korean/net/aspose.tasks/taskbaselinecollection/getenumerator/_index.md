---
title: "TaskBaselineCollection.GetEnumerator"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaselineCollection 메서드. 이 컬렉션에 대한 열거자를 반환합니다."
type: docs
weight: 40
url: /ko/net/aspose.tasks/taskbaselinecollection/getenumerator/
---
## TaskBaselineCollection.GetEnumerator method

이 컬렉션에 대한 열거자를 반환합니다.

```csharp
public IEnumerator<TaskBaseline> GetEnumerator()
```

### 반환 값

이 컬렉션에 대한 열거자.

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


