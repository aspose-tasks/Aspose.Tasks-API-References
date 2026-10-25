---
title: "Rsc.PeakUnits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. 리소스가 할당된 모든 작업에 대해 언제든지 리소스에 할당될 수 있는 최대 할당 단위"
type: docs
weight: 540
url: /ko/net/aspose.tasks/rsc/peakunits/
---
## Rsc.PeakUnits field

리소스가 할당된 모든 작업에 대해 언제든지 적용되는 최대 할당 단위입니다.

```csharp
public static readonly Key<double, RscKey> PeakUnits;
```

## 예제

Rsc.PeakUnits 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.PeakUnits, 2);

Console.WriteLine("Peak Units: " + resource.Get(Rsc.PeakUnits));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


