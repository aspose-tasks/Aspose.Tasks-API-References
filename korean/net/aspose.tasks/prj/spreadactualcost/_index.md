---
title: "Prj.SpreadActualCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Prj 필드. 실제 비용이 현재 상태 날짜에 반영되는지 여부를 결정합니다"
type: docs
weight: 660
url: /ko/net/aspose.tasks/prj/spreadactualcost/
---
## Prj.SpreadActualCost field

실제 비용이 상태 날짜까지 분배되는지 여부를 결정합니다.

```csharp
public static readonly Key<NullableBool, PrjKey> SpreadActualCost;
```

## 예제

Prj.SpreadActualCost 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

project.Set(Prj.SpreadActualCost, true);

Console.WriteLine("Spread Actual Cost: " + project.Get(Prj.SpreadActualCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


