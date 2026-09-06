---
title: "Prj.CurrencySymbol"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。项目中使用的货币符号。"
type: docs
weight: 170
url: /zh/net/aspose.tasks/prj/currencysymbol/
---
## Prj.CurrencySymbol field

项目中使用的货币符号。

```csharp
public static readonly Key<string, PrjKey> CurrencySymbol;
```

## 示例

展示如何写入项目的货币属性。

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// 设置货币属性
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// 显示货币属性
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### 另见

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


