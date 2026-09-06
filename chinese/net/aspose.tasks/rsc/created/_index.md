---
title: "Rsc.Created"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Rsc 字段。资源添加到项目的日期和时间"
type: docs
weight: 260
url: /zh/net/aspose.tasks/rsc/created/
---
## Rsc.Created field

资源添加到项目的日期和时间。

```csharp
public static readonly Key<DateTime, RscKey> Created;
```

## 示例

展示如何读取/写入 Rsc.Created 属性。

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Created, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Created: " + resource.Get(Rsc.Created));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


