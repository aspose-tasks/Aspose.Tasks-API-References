---
title: "Rsc.ActualOvertimeCost"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 할당된 리소스가 작업에 대해 이미 수행한 초과 근무에 발생한 비용"
type: docs
weight: 40
url: /ko/net/aspose.tasks/rsc/actualovertimecost/
---
## Rsc.ActualOvertimeCost field

할당된 리소스가 작업에서 이미 수행한 초과 근무에 대한 비용이 발생합니다.

```csharp
public static readonly Key<decimal, RscKey> ActualOvertimeCost;
```

## 예제

Rsc.ActualOvertimeCost 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + resource.Get(Rsc.ActualOvertimeCost));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


