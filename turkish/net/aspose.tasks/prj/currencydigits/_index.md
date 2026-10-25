---
title: "Prj.CurrencyDigits"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Ondalık sembolünden sonraki basamak sayısı"
type: docs
weight: 160
url: /tr/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

Ondalık sembolünden sonra gelen basamak sayısı.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
```

## Örnekler

Projenin para birimi özelliklerini nasıl yazacağınızı gösterir.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Para birimi özelliklerini ayarla
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Para birimi özelliklerini göster
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### Ayrıca Bakınız

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


