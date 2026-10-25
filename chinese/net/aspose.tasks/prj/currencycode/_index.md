---
title: "Prj.CurrencyCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "Prj 字段。根据 ISO 4217 定义的三字母货币字符代码。有效值示例为 USD。"
type: docs
weight: 150
url: /zh/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

ISO 4217 中定义的三字母货币代码。例如有效值为 "USD"。

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


