---
title: "Rsc.ActualCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 작업에서 이미 수행한 작업에 대해 발생한 비용과 해당 작업과 관련된 기타 기록된 비용"
type: docs
weight: 30
url: /ko/net/aspose.tasks/rsc/actualcost/
---
## Rsc.ActualCost field

리소스가 작업에서 이미 수행한 작업에 대한 비용과 작업과 관련된 기타 기록된 비용이 발생합니다.

```csharp
public static readonly Key<decimal, RscKey> ActualCost;
```

## 예제

Rsc.ActualCost 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualCost, 10m);

Console.WriteLine("Actual Cost: " + resource.Get(Rsc.ActualCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


