---
title: "Prj.CurrencySymbolPosition"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Prj veld. De plaatsing van het valutateken"
type: docs
weight: 180
url: /nl/net/aspose.tasks/prj/currencysymbolposition/
---
## Prj.CurrencySymbolPosition field

De plaatsing van het valutateken.

```csharp
public static readonly Key<CurrencySymbolPositionType, PrjKey> CurrencySymbolPosition;
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
* enum [CurrencySymbolPositionType](../../currencysymbolpositiontype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


