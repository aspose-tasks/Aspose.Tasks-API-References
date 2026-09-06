---
title: "Prj.DateFormat"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目视图日期格式"
type: docs
weight: 210
url: /zh/net/aspose.tasks/prj/dateformat/
---
## Prj.DateFormat field

项目视图日期格式。

```csharp
public static readonly Key<DateFormat, PrjKey> DateFormat;
```

## 示例

展示如何读取/写入 Prj.DateFormat 属性。

```csharp
var project = new Project();

project.Set(Prj.DateFormat, DateFormat.DateDd);

Console.WriteLine("Date Format: " + project.Get(Prj.DateFormat));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [DateFormat](../../dateformat/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


