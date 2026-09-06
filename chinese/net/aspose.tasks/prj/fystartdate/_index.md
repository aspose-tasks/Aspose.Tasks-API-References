---
title: "Prj.FyStartDate"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。财政年度开始的月份"
type: docs
weight: 350
url: /zh/net/aspose.tasks/prj/fystartdate/
---
## Prj.FyStartDate field

财政年度开始的月份。

```csharp
public static readonly Key<Month, PrjKey> FyStartDate;
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
* enum [Month](../../month/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


