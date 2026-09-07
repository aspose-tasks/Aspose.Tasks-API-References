---
title: "Prj.CurrencyCode"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il codice di tre lettere della valuta come definito in ISO 4217. Un esempio di valori validi è USD."
type: docs
weight: 150
url: /it/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

Il codice a tre lettere della valuta come definito in ISO 4217. Un esempio di valori validi è "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


