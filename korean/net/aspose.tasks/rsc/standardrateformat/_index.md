---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Rsc 필드. Microsoft Project에서 표준 요금을 표시하는 데 사용되는 단위"
type: docs
weight: 630
url: /ko/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Microsoft Project에서 표준 요율을 표시하는 데 사용되는 단위.

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## 예제

Rsc.StandardRateFormat 속성을 읽고 쓰는 방법을 보여줍니다.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


