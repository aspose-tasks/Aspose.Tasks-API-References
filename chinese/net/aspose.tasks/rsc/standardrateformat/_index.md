---
title: "Rsc.StandardRateFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。Microsoft Project 用于显示标准费率的单位"
type: docs
weight: 630
url: /zh/net/aspose.tasks/rsc/standardrateformat/
---
## Rsc.StandardRateFormat field

Microsoft Project 用于显示标准费率的单位。

```csharp
public static readonly Key<RateFormatType, RscKey> StandardRateFormat;
```

## 示例

展示如何读取/写入 Rsc.StandardRateFormat 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.StandardRateFormat, RateFormatType.Hour);

Console.WriteLine("Standard Rate Format: " + resource.Get(Rsc.StandardRateFormat));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateFormatType](../../rateformattype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


