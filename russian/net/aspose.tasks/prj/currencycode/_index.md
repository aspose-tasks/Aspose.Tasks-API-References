---
title: "Prj.CurrencyCode"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Поле Prj. Трёхбуквенный код валюты, определённый в ISO 4217. Пример допустимых значений: USD"
type: docs
weight: 150
url: /ru/net/aspose.tasks/prj/currencycode/
---
## Prj.CurrencyCode field

Трёхбуквенный код валюты, определённый в ISO 4217. Пример допустимого значения — "USD".

```csharp
public static readonly Key<string, PrjKey> CurrencyCode;
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


