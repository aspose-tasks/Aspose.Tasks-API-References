---
title: "Task.Baselines"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 속성. 작업의 기준값 컬렉션을 가져오거나 설정합니다"
type: docs
weight: 130
url: /ko/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

작업의 기준값 컬렉션을 가져오거나 설정합니다.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## 예제

작업의 기준값을 읽는 방법을 보여줍니다.

```csharp
var project = new Project();

// 기준값 설정
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 작업 베이스라인 지속 시간 표시
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### 또 보기

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


