---
title: "TaskBaseline.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaseline 메서드. 이 인스턴스가 지정된 TaskBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 100
url: /ko/net/aspose.tasks/taskbaseline/equals/
---
## Equals(TaskBaseline) {#equals_1}

이 인스턴스가 지정된 TaskBaseline 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(TaskBaseline other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | TaskBaseline | 이 인스턴스와 비교할 지정된 AssignmentBaseline 객체. |

### 반환 값

이 인스턴스가 지정된 TaskBaseline 객체와 같으면 true를 반환하고, 그렇지 않으면 false를 반환합니다.

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

---

## Equals(object) {#equals_2}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 객체. |

### 반환 값

**True** if the specified object is a TaskBaseline that has the same UID value as this instance; otherwise, **false**.

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


