---
title: "클래스 TaskBaseline"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.TaskBaseline 클래스. 작업의 기준선을 나타냅니다."
type: docs
weight: 2370
url: /ko/net/aspose.tasks/taskbaseline/
---
## TaskBaseline class

작업의 기준선(Baseline)을 나타냅니다.

```csharp
public sealed class TaskBaseline : Baseline, IComparable<TaskBaseline>, IEquatable<TaskBaseline>
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [TaskBaseline](taskbaseline/)(Task) | `TaskBaseline` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [BaselineNumber](../../aspose.tasks/baseline/baselinenumber/) { get; set; } | 베이스라인 데이터 레코드의 고유 번호를 가져오거나 설정합니다. |
| [Bcwp](../../aspose.tasks/baseline/bcwp/) { get; set; } | 프로젝트에 대해 리소스가 수행한 작업의 현재까지 예산 비용을 가져오거나 설정합니다. |
| [Bcws](../../aspose.tasks/baseline/bcws/) { get; set; } | 리소스에 예약된 작업의 예산 비용을 가져오거나 설정합니다. |
| [Cost](../../aspose.tasks/baseline/cost/) { get; set; } | 베이스라인이 저장될 때 리소스의 예상 비용을 가져오거나 설정합니다. |
| [Duration](../../aspose.tasks/taskbaseline/duration/) { get; set; } | 베이스라인이 저장될 때 작업의 예정 지속 시간을 가져오거나 설정합니다. |
| [EstimatedDuration](../../aspose.tasks/taskbaseline/estimatedduration/) { get; set; } | 작업의 베이스라인 지속 시간이 추정되었는지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Finish](../../aspose.tasks/taskbaseline/finish/) { get; set; } | 베이스라인이 저장될 때 작업의 예정 종료 날짜를 가져오거나 설정합니다. |
| [FixedCost](../../aspose.tasks/taskbaseline/fixedcost/) { get; set; } | 베이스라인이 저장될 때 작업의 고정 비용을 가져오거나 설정합니다. |
| [Interim](../../aspose.tasks/taskbaseline/interim/) { get; set; } | 이것이 중간 베이스라인인지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [Start](../../aspose.tasks/taskbaseline/start/) { get; set; } | 베이스라인이 저장될 때 작업의 예정 시작 날짜를 가져오거나 설정합니다. |
| [TimephasedData](../../aspose.tasks/taskbaseline/timephaseddata/) { get; set; } | `TimephasedDataCollection` 인스턴스를 이 객체에 대해 가져오거나 설정합니다. 작업 베이스라인과 연관된 시간 구분 데이터입니다. |
| [Work](../../aspose.tasks/baseline/work/) { get; set; } | 베이스라인이 저장될 때 리소스에 할당된 작업을 가져오거나 설정합니다. 베이스라인이 저장될 때 리소스에 할당된 작업량입니다. |

## 메서드

| 이름 | 설명 |
| --- | --- |
| [CompareTo](../../aspose.tasks/baseline/compareto/)(Baseline) | IComparable 인터페이스 구현입니다. 이 인스턴스를 지정된 Baseline 객체와 비교합니다. |
| [CompareTo](../../aspose.tasks/taskbaseline/compareto/#compareto_1)(TaskBaseline) | IComparable 인터페이스 구현입니다. 이 인스턴스를 지정된 Baseline 객체와 비교합니다. |
| [Equals](../../aspose.tasks/baseline/equals/)(Baseline) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [Equals](../../aspose.tasks/taskbaseline/equals/#equals_2)(object) | 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| [Equals](../../aspose.tasks/taskbaseline/equals/#equals_1)(TaskBaseline) | 이 인스턴스가 지정된 TaskBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다. |
| override [GetHashCode](../../aspose.tasks/taskbaseline/gethashcode/)() | `TaskBaseline` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다. |

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

* class [Baseline](../baseline/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


