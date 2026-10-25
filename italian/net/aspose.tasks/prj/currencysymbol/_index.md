---
title: "Prj.CurrencySymbol"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Campo Prj. Il simbolo della valuta usato in un progetto."
type: docs
weight: 170
url: /it/net/aspose.tasks/prj/currencysymbol/
---
## Prj.CurrencySymbol field

Il simbolo della valuta utilizzato in un progetto.

```csharp
public static readonly Key<string, PrjKey> CurrencySymbol;
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


