---
title: "Prj.CurrencySymbol"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj-veld. Het valutateken dat in een project wordt gebruikt."
type: docs
weight: 170
url: /nl/net/aspose.tasks/prj/currencysymbol/
---
## Prj.CurrencySymbol field

Het valutateken dat in een project wordt gebruikt.

```csharp
public static readonly Key<string, PrjKey> CurrencySymbol;
```

## Voorbeelden

Toont hoe de valutaproperties van het project te schrijven.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Stel valutaproperties in
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Toon valutaproperties
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Zie ook

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


