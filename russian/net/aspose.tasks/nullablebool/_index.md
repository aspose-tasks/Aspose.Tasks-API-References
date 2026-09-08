---
title: "Структура NullableBool"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Структура Aspose.Tasks.NullableBool. Класс для булевых значений с возможностью проверить, было ли значение определено или нет."
type: docs
weight: 1110
url: /ru/net/aspose.tasks/nullablebool/
---
## NullableBool structure

Класс для логических значений с возможностью проверить, было ли значение определено.

```csharp
public struct NullableBool : IEquatable<NullableBool>
```

## Конструкторы

| Имя | Описание |
| --- | --- |
| [NullableBool](nullablebool/#constructor)(bool) | Инициализирует новый экземпляр структуры `NullableBool` с указанным булевым значением. |
| [NullableBool](nullablebool/#constructor_1)(bool, bool) | Инициализирует новый экземпляр структуры `NullableBool`. |

## Свойства

| Имя | Описание |
| --- | --- |
| [IsDefined](../../aspose.tasks/nullablebool/isdefined/) { get; } | Возвращает значение, указывающее, было ли значение определено; в противном случае — false. |
| [Value](../../aspose.tasks/nullablebool/value/) { get; set; } | Получает или задает значение, указывающее, является ли текущее значение true или false. |

## Методы

| Имя | Описание |
| --- | --- |
| [Equals](../../aspose.tasks/nullablebool/equals/#equals)(NullableBool) | Возвращает флаг, указывающий, равен ли этот экземпляр указанному экземпляру класса `NullableBool`. |
| override [Equals](../../aspose.tasks/nullablebool/equals/#equals_1)(object) | Возвращает флаг, указывающий, равен ли этот экземпляр указанному объекту. |
| override [GetHashCode](../../aspose.tasks/nullablebool/gethashcode/)() | Возвращает значение хеш‑кода для экземпляра класса `NullableBool`. |
| override [ToString](../../aspose.tasks/nullablebool/tostring/)() | Возвращает строку, представляющую текущий объект. |
| [operator ==](../../aspose.tasks/nullablebool/op_equality/) | Возвращает значение, указывающее, равен ли этот экземпляр указанному объекту. |
| [implicit operator](../../aspose.tasks/nullablebool/op_implicit/#op_implicit_1) | Неявно преобразует экземпляр `NullableBool` в логическое значение. Возвращает true, когда [`Value`](./value/) равно true и [`IsDefined`](./isdefined/) равно true. (2 оператора) |
| [operator !=](../../aspose.tasks/nullablebool/op_inequality/) | Возвращает значение, указывающее, не равен ли этот экземпляр указанному объекту. |

## Примеры

Показывает, как работать с классом &lt;see cref="NullableBool" /&gt;.

```csharp
var project = new Project();

// Проверим, где используется класс <see cref="Aspose.Tasks.NullableBool" />.
// Главное преимущество <see cref="Aspose.Tasks.NullableBool" /> заключается в том, что 
// Можно установить его как неопределённый при создании.
var actualsInSync = new NullableBool(false, false);
Console.WriteLine("'ActualsInSync' Value: " + actualsInSync.Value);
Console.WriteLine("'ActualsInSync' Is Defined: " + actualsInSync.IsDefined);

// ...
// использовать экземпляр nullable bool
project.Set(Prj.ActualsInSync, actualsInSync);

// ...
var honorConstraints = new NullableBool(true);
Console.WriteLine("'HonorConstraints' ToString: " + honorConstraints.ToString());

// ...
// использовать экземпляр nullable bool
project.Set(Prj.HonorConstraints, honorConstraints);

// ...
```

### См. также

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


