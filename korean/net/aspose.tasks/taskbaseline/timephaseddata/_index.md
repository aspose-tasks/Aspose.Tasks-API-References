---
title: "TaskBaseline.TimephasedData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaseline 속성. 이 객체에 대한 TimephasedDataCollection 인스턴스를 가져오거나 설정합니다. 작업 기준선과 연결된 시간 단계 데이터"
type: docs
weight: 80
url: /ko/net/aspose.tasks/taskbaseline/timephaseddata/
---
## TaskBaseline.TimephasedData property

`TimephasedDataCollection` 인스턴스를 이 객체에 대해 가져오거나 설정합니다. 작업 베이스라인과 연관된 시간 구분 데이터입니다.

```csharp
public TimephasedDataCollection TimephasedData { get; set; }
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

* class [TimephasedDataCollection](../../timephaseddatacollection/)
* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


