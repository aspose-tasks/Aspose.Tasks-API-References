---
title: "NullableBool.ToString"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод NullableBool. Возвращает строку, представляющую текущий объект"
type: docs
weight: 60
url: /ru/net/aspose.tasks/nullablebool/tostring/
---
## NullableBool.ToString method

Возвращает строку, представляющую текущий объект.

```csharp
public override string ToString()
```

### Возвращаемое значение

Строка, представляющая текущий объект.

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


