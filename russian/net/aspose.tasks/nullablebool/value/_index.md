---
title: "NullableBool.Value"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство NullableBool. Получает или задает значение, указывающее, является ли текущее значение истинным или ложным"
type: docs
weight: 30
url: /ru/net/aspose.tasks/nullablebool/value/
---
## NullableBool.Value property

Получает или задает значение, указывающее, является ли текущее значение true или false.

```csharp
public bool Value { get; set; }
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


