---
title: "Metered.SetMeteredKey"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Metered method. Устанавливает публичные и приватные ключи Metered"
type: docs
weight: 40
url: /ru/net/aspose.tasks/metered/setmeteredkey/
---
## Metered.SetMeteredKey method

Устанавливает публичные и приватные метерные ключи.

```csharp
public void SetMeteredKey(string publicKey, string privateKey)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| publicKey | Строка | Публичный ключ. |
| privateKey | Строка | Закрытый ключ. |

## Примечания

Если вы приобретаете лицензию с измерением, этот API должен вызываться при запуске приложения, обычно этого достаточно. Однако, если измерение не удаётся загрузить данные о потреблении в течение 24‑часового периода, лицензия будет переведена в статус оценки. Чтобы избежать такой ситуации, следует регулярно проверять статус лицензии. Если статус — оценочный, вызовите этот API снова.

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


