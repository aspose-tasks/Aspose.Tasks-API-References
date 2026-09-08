---
title: "TaskLink.Equals"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskLink 메서드. 이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다"
type: docs
weight: 90
url: /ko/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public bool Equals(TaskLink other)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| other | TaskLink | 이 인스턴스와 비교할 지정된 [`TaskLink`](../) 클래스 인스턴스입니다. |

### 반환 값

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## 예제

작업 링크의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// 작업 링크의 동일성은 선행 및 후속 작업을 기반으로 합니다.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### 또 보기

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

이 인스턴스가 지정된 객체와 같은지 여부를 나타내는 값을 반환합니다.

```csharp
public override bool Equals(object obj)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| obj | Object | 이 인스턴스와 비교할 객체. |

### 반환 값

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## 예제

작업 링크의 동일성을 확인하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// 작업 링크의 동일성은 선행 및 후속 작업을 기반으로 합니다.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### 또 보기

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


