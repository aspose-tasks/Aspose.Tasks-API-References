---
title: "Task.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Task 메서드. 이 인스턴스가 지정된 작업과 같은지 여부를 나타내는 값을 반환합니다."
type: docs
weight: 1330
url: /ko/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

이 인스턴스가 지정된 작업과 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(Task other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 다른 | 작업 | 이 인스턴스와 비교할 지정된 작업. |

### 반환 값

지정된 작업과 이 인스턴스가 동일한 고유 ID를 가지고 있으면 true를 반환합니다.

## 예제

작업 할당을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 작업 할당을 표시합니다.
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 지정된 객체. |

### 반환 값

지정된 작업과 이 인스턴스가 동일한 고유 ID를 가지고 있으면 true를 반환합니다.

## 예제

작업 할당을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // 작업 할당을 표시합니다.
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### 또 보기

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


