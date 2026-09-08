---
title: "Metered.ResetMeteredKey"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод Metered. Удаляет ранее настроенную лицензию"
type: docs
weight: 30
url: /ru/net/aspose.tasks/metered/resetmeteredkey/
---
## Metered.ResetMeteredKey method

Удаляет ранее настроенную лицензию.

```csharp
public void ResetMeteredKey()
```

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


