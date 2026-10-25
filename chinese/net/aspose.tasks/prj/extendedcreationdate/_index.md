---
title: "Prj.ExtendedCreationDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。用于计算和报告的日期"
type: docs
weight: 320
url: /zh/net/aspose.tasks/prj/extendedcreationdate/
---
## Prj.ExtendedCreationDate field

用于计算和报告的日期。

```csharp
public static readonly Key<DateTime, PrjKey> ExtendedCreationDate;
```

## 示例

展示如何读取/写入 Prj.ExtendedCreationDate 属性。

```csharp
var project = new Project();

project.Set(Prj.ExtendedCreationDate, new DateTime(2020, 4, 10, 9, 0, 0));

Console.WriteLine("Extended Creation Date: " + project.Get(Prj.ExtendedCreationDate));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


