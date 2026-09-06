---
title: "Rsc.AvailableFrom"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段. 资源在当前时间段指定的单位下可工作的开始日期."
type: docs
weight: 120
url: /zh/net/aspose.tasks/rsc/availablefrom/
---
## Rsc.AvailableFrom field

资源在当前时间段内按指定单位可工作的开始日期。

```csharp
public static readonly Key<DateTime, RscKey> AvailableFrom;
```

## 示例

展示如何读取/写入 Rsc.AvailableFrom 属性.

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.AvailableFrom, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Available From: " + resource.Get(Rsc.AvailableFrom));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


