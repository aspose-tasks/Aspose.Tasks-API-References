---
title: "Rsc.RemainingCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 남은 예정 작업을 완료하는 데 발생할 남은 예정 비용"
type: docs
weight: 580
url: /ko/net/aspose.tasks/rsc/remainingcost/
---
## Rsc.RemainingCost field

남은 예정 작업을 완료하는 데 발생할 남은 예정 비용.

```csharp
public static readonly Key<decimal, RscKey> RemainingCost;
```

## 예제

Rsc.RemainingCost 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.RemainingCost, 2);

Console.WriteLine("Remaining Cost: " + resource.Get(Rsc.RemainingCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


