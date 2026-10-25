---
title: "Classe EntityFieldAttribute"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Classe Aspose.Tasks.Attributes.EntityFieldAttribute. Représente un attribut pour les propriétés d'entité"
type: docs
weight: 70
url: /fr/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Représente un attribut pour les propriétés d'entité.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Constructeurs

| Nom | Description |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Le constructeur par défaut. |

## Remarques

Attribut utilisé uniquement pour les propriétés d'entité [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) et [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), et simplifie son énumération.

## Exemples

Comment énumérer les propriétés en utilisant l'attribut **EntityField** :

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

### Voir aussi

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


