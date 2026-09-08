---
title: "TaskBaseline.GetHashCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "TaskBaseline 메서드. TaskBaseline 클래스 인스턴스에 대한 해시 코드 값을 반환합니다."
type: docs
weight: 110
url: /ko/net/aspose.tasks/taskbaseline/gethashcode/
---
## TaskBaseline.GetHashCode method

`[`TaskBaseline`](../)` 클래스 인스턴스에 대한 해시 코드 값을 반환합니다.

```csharp
public override int GetHashCode()
```

### 반환 값

이 객체에 대한 해시 코드 값을 반환합니다.

## 예제

작업 기준선의 해시 코드를 가져오는 방법을 보여줍니다.

```csharp
var project = new Project();

// TaskBaseline 생성
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// 작업 베이스라인 기간을 표시
var baseline1 = task.Baselines.ToList()[0];
var baseline2 = task.Baselines.ToList()[0];

// 캘린더의 해시 코드는 기준선 번호와 같습니다.
Console.WriteLine("Baseline 1 Number: {0} Hash Code: {1}", (int)baseline1.BaselineNumber, baseline1.GetHashCode());
Console.WriteLine("Baseline 2 Number: {0} Hash Code: {1}", (int)baseline2.BaselineNumber, baseline2.GetHashCode());
```

### 또 보기

* class [TaskBaseline](../)
* namespace [Aspose.Tasks](../../taskbaseline/)
* assembly [Aspose.Tasks](../../../)


