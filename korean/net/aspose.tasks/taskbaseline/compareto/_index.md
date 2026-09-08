---
title: "TaskBaseline.CompareTo"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaseline 메서드. IComparable 인터페이스 구현. 이 인스턴스를 지정된 Baseline 객체와 비교합니다"
type: docs
weight: 90
url: /ko/net/aspose.tasks/taskbaseline/compareto/
---
## TaskBaseline.CompareTo method

IComparable 인터페이스 구현입니다. 이 인스턴스를 지정된 Baseline 객체와 비교합니다.

```csharp
public int CompareTo(TaskBaseline other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | TaskBaseline | 이 인스턴스를 비교할 지정된 Baseline 객체. |

### 반환 값

이 인스턴스가 지정된 객체보다 작으면 -1을 반환하고, 크면 1을 반환합니다; 그 외의 경우 0을 반환합니다.

## 예제

베이스라인의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project();

// TaskBaseline 생성
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 작업 베이스라인 기간을 표시
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// 베이스라인의 동일성은 베이스라인 숫자와 비교하여 확인됩니다.
Console.WriteLine("Baseline Number 1: " + baseline1.BaselineNumber);
Console.WriteLine("Baseline Number 2: " + baseline2.BaselineNumber);
Console.WriteLine("Are baselines equal: " + baseline1.Equals(baseline2));
```

### 또 보기

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


