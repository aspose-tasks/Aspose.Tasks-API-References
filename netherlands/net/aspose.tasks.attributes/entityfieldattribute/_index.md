---
title: "Klasse EntityFieldAttribute"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Aspose.Tasks.Attributes.EntityFieldAttribute class. Vertegenwoordigt een attribuut voor entiteitseigenschappen"
type: docs
weight: 70
url: /nl/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Stelt een attribuut voor entiteitseigenschappen voor.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Constructors

| Naam | Beschrijving |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | De standaardconstructor. |

## Opmerkingen

Attribuut dat alleen wordt gebruikt voor [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) en [`ResourceAssignment`](../../aspose.tasks/resourceassignment/) entiteitseigenschappen, en vereenvoudigt de enumeratie ervan.

## Voorbeelden

Hoe eigenschappen te enumereren met behulp van het **EntityField** attribuut:

```csharp
[C#]
var project = new Project("sample.mpp");
foreach (var task in project.SelectAllChildTasks())
{
    Console.WriteLine("Task:");
    foreach (var propInfo in typeof(Task).GetProperties().Where(propInfo => propInfo.GetCustomAttribute{Attributes.EntityFieldAttribute}() != null))
    {
        Console.WriteLine(string.Format("{0}: {1}", propInfo.Name, propInfo.GetValue(task)));
    }
}
```

### Zie ook

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


