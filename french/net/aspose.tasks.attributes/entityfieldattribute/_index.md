---
title: Class EntityFieldAttribute
second_title: Référence de l'API Aspose.Tasks pour .NET
description: Aspose.Tasks.Attributes.EntityFieldAttribute classe. Représente un attribut pour les propriétés dentité.
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

| Nom | La description |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Constructor |

### Remarques

Attribut utilisé pour[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) et[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) propriétés d'entité uniquement et simplifie son énumération.

### Exemples

Comment énumérer les propriétés en utilisant **EntityField** attribut :

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

### Voir également

* espace de noms [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* Assemblée [Aspose.Tasks](../../)


