---
title: "Rsc.MaxUnits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 현재 기간 동안 리소스가 작업을 수행할 수 있는 최대 용량을 나타내는 최대 단위 수"
type: docs
weight: 450
url: /ko/net/aspose.tasks/rsc/maxunits/
---
## Rsc.MaxUnits field

리소스가 현재 기간 동안 모든 작업을 수행할 수 있는 최대 용량을 나타내는 최대 단위 수입니다.

```csharp
public static readonly Key<double, RscKey> MaxUnits;
```

## 예제

Rsc.MaxUnits 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.MaxUnits, 2);

Console.WriteLine("Max Units: " + resource.Get(Rsc.MaxUnits));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


