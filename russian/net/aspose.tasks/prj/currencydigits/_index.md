---
title: "Prj.CurrencyDigits"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Prj field. Количество цифр после десятичного знака"
type: docs
weight: 160
url: /ru/net/aspose.tasks/prj/currencydigits/
---
## Prj.CurrencyDigits field

Количество цифр после десятичного разделителя.

```csharp
public static readonly Key<int, PrjKey> CurrencyDigits;
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
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


