---
title: "Prj.CurrencySymbolPosition"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Prj alanı. Para birimi simgesinin konumu"
type: docs
weight: 180
url: /tr/net/aspose.tasks/prj/currencysymbolposition/
---
## Prj.CurrencySymbolPosition field

Para birimi simgesinin konumu.

```csharp
public static readonly Key<CurrencySymbolPositionType, PrjKey> CurrencySymbolPosition;
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
* enum [CurrencySymbolPositionType](../../currencysymbolpositiontype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


