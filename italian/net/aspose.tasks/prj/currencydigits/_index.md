---
title: "Prj.CurrencyDigits"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il numero di cifre dopo il simbolo decimale"
type: docs
weight: 160
url: /it/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

Il numero di cifre dopo il simbolo decimale.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## Esempi

Mostra come scrivere le proprietà di valuta del progetto.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Imposta le proprietà di valuta
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Visualizza le proprietà di valuta
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Vedi anche

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


