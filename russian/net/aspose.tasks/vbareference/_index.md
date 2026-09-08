---
title: "Класс VbaReference"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Класс Aspose.Tasks.VbaReference. Представляет ссылку на VbaProject."
type: docs
weight: 2870
url: /ru/net/aspose.tasks/vbareference/
---
## VbaReference class

Представляет ссылку на [`VbaProject`](../vbaproject/).

```csharp
public sealed class VbaReference : IEquatable<VbaReference>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [VbaReference](vbareference/)() | Конструктор по умолчанию. |

## Свойства

| Имя | Описание |
| --- | --- |
| [LibIdentifier](../../aspose.tasks/vbareference/libidentifier/) { get; } | Получает идентификатор библиотеки. |
| [Name](../../aspose.tasks/vbareference/name/) { get; set; } | Получает или задает имя VBA‑ссылки. |

## Методы

| Имя | Описание |
| --- | --- |
| override [Equals](../../aspose.tasks/vbareference/equals/#equals_1)(object) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту `VbaReference`. |
| [Equals](../../aspose.tasks/vbareference/equals/#equals)(VbaReference) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту `VbaReference`. |
| override [GetHashCode](../../aspose.tasks/vbareference/gethashcode/)() | Возвращает значение хэш‑кода для этого `VbaReference`. |

## Примеры

Показывает, как читать VBA‑ссылки.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Reference count " + project.VbaProject.References.Count);

foreach (var reference in project.VbaProject.References)
{
    Console.WriteLine("Identifier: " + reference.LibIdentifier);
    Console.WriteLine("Name: " + reference.Name);
}
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


