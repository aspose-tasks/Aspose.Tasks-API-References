---
title: Prj.CurrencyDigits
second_title: Aspose.Tasks for .NET API Reference
description: Prj field. The number of digits after a decimal symbol
type: docs
weight: 160
url: /net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

The number of digits after a decimal symbol.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## Examples

Shows how to write project's currency properties.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Set currency properties
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Display currency properties
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### See Also

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


