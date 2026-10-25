---
title: "Класс Metered"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.Metered. Предоставляет методы для установки метерного ключа"
type: docs
weight: 1020
url: /ru/net/aspose.tasks/metered/
---
## Metered class

Предоставляет методы для установки измеряемого ключа.

```csharp
public class Metered
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [Metered](metered/)() | Конструктор по умолчанию. |

## Методы

| Имя | Описание |
| --- | --- |
| [IsLicensed](../../aspose.tasks/metered/islicensed/)() | Проверяет, успешно ли продукт лицензирован с использованием метерной лицензии. |
| [ResetMeteredKey](../../aspose.tasks/metered/resetmeteredkey/)() | Удаляет ранее настроенную лицензию. |
| [SetMeteredKey](../../aspose.tasks/metered/setmeteredkey/)(string, string) | Устанавливает публичные и приватные метерные ключи. |
| static [GetConsumptionCredit](../../aspose.tasks/metered/getconsumptioncredit/)() | Получает кредит потребления. |
| static [GetConsumptionQuantity](../../aspose.tasks/metered/getconsumptionquantity/)() | Получает размер файла потребления. |

## Примеры

В этом примере будет предпринята попытка установить публичный и приватный метерный ключ

```csharp
[C#]

Metered metered = new Metered();
metered.SetMeteredKey("PublicKey", "PrivateKey");


[Visual Basic]

Dim metered As Metered = New Metered
metered.SetMeteredKey("PublicKey", "PrivateKey")
```

файл jar компонента:

```csharp
Metered metered = new Metered();
metered.setMeteredKey("PublicKey", "PrivateKey");
```

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


