---
title: "Metered.GetConsumptionQuantity"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Metered. Получает размер файла потребления"
type: docs
weight: 60
url: /ru/net/aspose.tasks/metered/getconsumptionquantity/
---
## Metered.GetConsumptionQuantity method

Получает размер файла потребления.

```csharp
public static decimal GetConsumptionQuantity()
```

### Возвращаемое значение

Возвращает количество потреблённых байт.

## Примеры

Показывает, как использовать &lt;see cref="Aspose.Tasks.Metered" /&gt; тип лицензии с Aspose.Tasks.

```csharp
// Давайте используем лицензию с учётом потребления (see https://purchase.aspose.com/faqs/licensing/metered)
// установить лицензию с учётом потребления
var metered = new Metered();
metered.SetMeteredKey("<public key>", "<private key>");

var project = new Project(DataDir + "Project2.mpp");
Console.WriteLine("Project Name: " + project.Get(Prj.Name));

// ...
// работать с проектом...
// ...

// Мы можем получить текущие кредиты и потребление байтов.

try
{
    Console.WriteLine("Credits spent: {0}", Metered.GetConsumptionCredit());
    Console.WriteLine("Bytes consumed: {0}", Metered.GetConsumptionQuantity());
}
catch (WebException)
{
    // записать исключение
}

// в последнее время пользователь может сбросить учёт потребления и остановить подсчёт байтов
metered.ResetMeteredKey();
```

### См. также

* class [Metered](../)
* namespace [Aspose.Tasks](../../metered/)
* assembly [Aspose.Tasks](../../../)


