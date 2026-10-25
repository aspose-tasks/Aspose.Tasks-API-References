---
title: "Rsc.CostPerUse"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 사용될 때마다 발생하는 비용"
type: docs
weight: 240
url: /ko/net/aspose.tasks/rsc/costperuse/
---
## Rsc.CostPerUse field

리소스가 사용될 때마다 발생하는 비용.

```csharp
public static readonly Key<decimal, RscKey> CostPerUse;
```

## 예제

Rsc.CostPerUse 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostPerUse, 9);

Console.WriteLine("Cost Per Use: " + resource.Get(Rsc.CostPerUse));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


