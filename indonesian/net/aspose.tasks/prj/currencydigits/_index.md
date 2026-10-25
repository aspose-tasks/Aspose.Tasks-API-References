---
title: "Prj.CurrencyDigits"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Prj field. Jumlah digit setelah simbol desimal"
type: docs
weight: 160
url: /id/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

Jumlah digit setelah simbol desimal.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## Contoh

Menampilkan cara menulis properti mata uang proyek.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Atur properti mata uang
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Tampilkan properti mata uang
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


