---
title: "Rsc.CostVariance"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스의 기준 비용과 총 비용 간의 차이"
type: docs
weight: 250
url: /ko/net/aspose.tasks/rsc/costvariance/
---
## Rsc.CostVariance field

리소스의 기준 비용과 총 비용 간의 차이.

```csharp
public static readonly Key<double, RscKey> CostVariance;
```

## 예제

Rsc.CostVariance 속성을 읽고/쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.CostVariance, 10);

Console.WriteLine("Cost Variance: " + resource.Get(Rsc.CostVariance));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


