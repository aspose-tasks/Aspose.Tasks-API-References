---
title: "NullableBool.IsDefined"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство NullableBool. Возвращает значение, указывающее, было ли значение определено, иначе false"
type: docs
weight: 20
url: /ru/net/aspose.tasks/nullablebool/isdefined/
---
## NullableBool.IsDefined property

Возвращает значение, указывающее, было ли значение определено; в противном случае — false.

```csharp
public bool IsDefined { get; }
```

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


