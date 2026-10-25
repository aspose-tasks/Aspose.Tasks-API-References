---
title: "Prj.CustomDateFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目视图自定义日期格式。当 DateFormat 属性设置为 Custom 时用于格式化日期"
type: docs
weight: 200
url: /zh/net/aspose.tasks/prj/customdateformat/
---
## Prj.CustomDateFormat field

项目视图自定义日期格式。当 [`DateFormat`](../dateformat/) 属性设置为 Custom 时用于格式化日期。

```csharp
public static readonly Key<string, PrjKey> CustomDateFormat;
```

## 示例

展示如何读取/写入 Prj.CustomDateFormat 属性。

```csharp
var project = new Project();

project.Set(Prj.CustomDateFormat, "dd MMMM yyyy H:mm");

Console.WriteLine("Custom Date Format: " + project.Get(Prj.CustomDateFormat));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


