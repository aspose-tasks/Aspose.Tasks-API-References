---
title: "Asn.CostRateTableType"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 이 할당에 사용되는 비용 요율 표"
type: docs
weight: 190
url: /ko/net/aspose.tasks/asn/costratetabletype/
---
## Asn.CostRateTableType field

이 과제에 사용되는 비용률 표.

```csharp
public static readonly Key<RateType, AsnKey> CostRateTableType;
```

## 예제

Asn.CostRateTableType 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.CostRateTableType, RateType.B);

Console.WriteLine("Cost Rate Table Type: " + assignment.Get(Asn.CostRateTableType));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateType](../../ratetype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


