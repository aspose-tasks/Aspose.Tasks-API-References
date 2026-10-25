---
title: "Prj.FiscalYearStart"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。确定是否使用财政年度编号"
type: docs
weight: 340
url: /zh/net/aspose.tasks/prj/fiscalyearstart/
---
## Prj.FiscalYearStart field

确定是否使用财政年度编号。

```csharp
public static readonly Key<NullableBool, PrjKey> FiscalYearStart;
```

## 示例

展示如何编写财政年度属性。

```csharp
var project = new Project(DataDir + "WriteFiscalYearProperties.mpp");

// 设置财政年度属性
project.Set(Prj.FyStartDate, Month.July);
project.Set(Prj.FiscalYearStart, true);

// 显示财政年度属性
Console.WriteLine("Fiscal Year Start Date: " + project.Get(Prj.FyStartDate));
Console.WriteLine("Fiscal Year Numbering: " + project.Get(Prj.FiscalYearStart));
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


