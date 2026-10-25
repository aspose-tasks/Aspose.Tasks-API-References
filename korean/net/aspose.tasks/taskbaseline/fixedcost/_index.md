---
title: "TaskBaseline.FixedCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaseline 속성. 기준선이 저장될 때 작업의 고정 비용을 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/taskbaseline/fixedcost/
---
## TaskBaseline.FixedCost property

베이스라인이 저장될 때 작업의 고정 비용을 가져오거나 설정합니다.

```csharp
public double FixedCost { get; set; }
```

## 예제

베이스라인 정보에 접근하는 방법을 보여줍니다.

```csharp
var project = new Project();

// TaskBaseline 생성
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 작업 베이스라인 지속 시간 표시
var baseline = task.Baselines.ToList()[0];
Console.WriteLine("Baseline Start: {0}", baseline.Start);
Console.WriteLine("Baseline duration: {0}", baseline.Duration);
Console.WriteLine("Baseline duration format: {0}", baseline.Duration.TimeUnit);
Console.WriteLine("Is it estimated duration?: {0}", baseline.EstimatedDuration);
Console.WriteLine("Baseline Finish: {0}", baseline.Finish);

// 이것이 중간 베이스라인인지 여부를 나타내는 값
Console.WriteLine("Interim: {0}", baseline.Interim);
Console.WriteLine("Fixed Cost: {0}", baseline.FixedCost);

// 작업 베이스라인의 시간 구분 데이터를 출력합니다
Console.WriteLine("Number of timephased items: " + baseline.TimephasedData.Count);
foreach (var data in baseline.TimephasedData)
{
    Console.WriteLine(" Uid: " + data.Uid);
    Console.WriteLine(" Start: " + data.Start);
    Console.WriteLine(" Finish: " + data.Finish);
}
```

### 또 보기

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


