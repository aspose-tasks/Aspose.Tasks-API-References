---
title: "Prj.CurrencyCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Kode karakter mata uang tiga huruf sebagaimana didefinisikan dalam ISO 4217. Contoh nilai yang valid adalah USD"
type: docs
weight: 150
url: /id/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

Kode karakter mata uang tiga huruf sebagaimana didefinisikan dalam ISO 4217. Contoh nilai yang valid adalah "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


