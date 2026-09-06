---
title: "Prj.LastPrinted"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目的最后打印时间。以 UTC 格式保存在 mpp 文件中。DateTime 类型"
type: docs
weight: 430
url: /zh/net/aspose.tasks/prj/lastprinted/
---
## Prj.LastPrinted field

项目的最后打印时间。以 UTC 格式保存在 mpp 文件中。DateTime 类型。

```csharp
public static readonly Key<DateTime, PrjKey> LastPrinted;
```

## 示例

展示如何读取/写入 Prj.LastPrinted 属性。

```csharp
var project = new Project();

project.Set(Prj.LastPrinted, new DateTime(2020, 4, 10, 13, 0, 0));

Console.WriteLine("Last Printed: " + project.Get(Prj.LastPrinted));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


