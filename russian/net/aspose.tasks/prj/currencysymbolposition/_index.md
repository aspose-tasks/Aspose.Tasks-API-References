---
title: "Prj.CurrencySymbolPosition"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Расположение символа валюты"
type: docs
weight: 180
url: /ru/net/aspose.tasks/prj/currencysymbolposition/
---
## Prj.CurrencySymbolPosition field

Размещение символа валюты.

```csharp
public static readonly Key<CurrencySymbolPositionType, PrjKey> CurrencySymbolPosition;
```

## Примеры

Показывает, как записать свойства валюты проекта.

```csharp
var project = new Project(DataDir + "WriteCurrencyProperties.mpp");

// Установить свойства валюты
project.Set(Prj.CurrencyCode, "AUD");
project.Set(Prj.CurrencyDigits, 2);
project.Set(Prj.CurrencySymbol, "$");
project.Set(Prj.CurrencySymbolPosition, CurrencySymbolPositionType.After);

// Отобразить свойства валюты
Console.WriteLine("Currency Code: " + project.Get(Prj.CurrencyCode));
Console.WriteLine("Currency Digits: " + project.Get(Prj.CurrencyDigits));
Console.WriteLine("Currency Symbol: " + project.Get(Prj.CurrencySymbol));
Console.WriteLine("Currency Symbol Position: " + project.Get(Prj.CurrencySymbolPosition));

project.Save(OutDir + "WriteCurrencyProperties_out.xml", SaveFileFormat.Xml);
```

### См. также

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [CurrencySymbolPositionType](../../currencysymbolpositiontype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


