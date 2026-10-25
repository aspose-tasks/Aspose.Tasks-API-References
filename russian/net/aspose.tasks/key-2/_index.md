---
title: "Структура KeyTK"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Структура Aspose.Tasks.Key2TK. Представляет ключ свойства класса указанного типа. Экземпляр этого класса используется при получении или установке свойства контейнера"
type: docs
weight: 930
url: /ru/net/aspose.tasks/key-2/
---
## Key&lt;T,K&gt; structure

Представляет ключ свойства класса указанного типа. Экземпляр этого класса используется при получении или установке свойства контейнера.

```csharp
public struct Key<T, K>
    where K : struct
```

| Параметр | Описание |
| --- | --- |
| T | Тип значения свойства. |
| K | Тип ключа свойства. |

## Свойства

| Имя | Описание |
| --- | --- |
| [KeyType](../../aspose.tasks/key-2/keytype/) { get; } | Получает ключ свойства. |

## Примеры

Показывает, как читать/записывать свойство Prj.ActualsInSync.

```csharp
var project = new Project();

project.Set(Prj.ActualsInSync, true);

Console.WriteLine("Actuals In Sync: " + project.Get(Prj.ActualsInSync));
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


