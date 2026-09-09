---
title: "Prj.CurrencyCode"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alan. ISO 4217'de tanımlanan üç harfli para birimi kodu. Geçerli değer örneği USD."
type: docs
weight: 150
url: /tr/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

ISO 4217'de tanımlanan üç harfli para birimi kodu. Geçerli değer örneği "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


