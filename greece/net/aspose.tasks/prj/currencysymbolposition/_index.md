---
title: "Prj.CurrencySymbolPosition"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Η θέση του συμβόλου του νομίσματος"
type: docs
weight: 180
url: /el/net/aspose.tasks/prj/currencysymbolposition/
---
## Prj.CurrencySymbolPosition field

Η θέση του συμβόλου νομίσματος.

```csharp
public static readonly Key<CurrencySymbolPositionType, PrjKey> CurrencySymbolPosition;
```

## Παραδείγματα

Δείχνει πώς να γράψετε τις ιδιότητες νομίσματος του έργου.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Ορίστε ιδιότητες νομίσματος
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Εμφανίστε ιδιότητες νομίσματος
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CurrencySymbolPositionType](../../currencysymbolpositiontype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


