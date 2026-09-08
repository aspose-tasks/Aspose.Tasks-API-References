---
title: "NullableBool.NullableBool"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Конструктор NullableBool. Инициализирует новый экземпляр структуры NullableBool с указанным логическим значением"
type: docs
weight: 10
url: /ru/net/aspose.tasks/nullablebool/nullablebool/
---
## NullableBool(bool) {#constructor}

Инициализирует новый экземпляр структуры [`NullableBool`](../) с указанным логическим значением.

```csharp
public NullableBool(bool value)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| value | Boolean | указанное логическое значение. |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)

---

## NullableBool(bool, bool) {#constructor_1}

Инициализирует новый экземпляр структуры [`NullableBool`](../).

```csharp
public NullableBool(bool value, bool isDefined)
```

| Параметр | Тип | Описание |
| --- | --- | --- |
| value | Boolean | Текущее значение. |
| isDefined | Boolean | Значение, указывающее, определено ли текущее значение. |

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

* struct [NullableBool](../)
* namespace [Aspose.Tasks](../../nullablebool/)
* assembly [Aspose.Tasks](../../../)


