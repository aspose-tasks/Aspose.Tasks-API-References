---
title: "Prj.CurrencyCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Πεδίο Prj. Ο τριψήφιος κωδικός νομίσματος όπως ορίζεται στο ISO 4217. Παράδειγμα έγκυρων τιμών είναι USD."
type: docs
weight: 150
url: /el/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

Ο τριψήφιος κωδικός νομίσματος όπως ορίζεται στο ISO 4217. Παράδειγμα έγκυρης τιμής είναι "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


