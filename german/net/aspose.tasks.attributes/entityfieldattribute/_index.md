---
title: Class EntityFieldAttribute
second_title: Aspose.Tasks für .NET-API-Referenz
description: Aspose.Tasks.Attributes.EntityFieldAttribute klas. Stellt ein Attribut für Entitätseigenschaften dar.
type: docs
weight: 70
url: /de/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Stellt ein Attribut für Entitätseigenschaften dar.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Konstrukteure

| Name | Beschreibung |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Constructor |

### Bemerkungen

Attribut verwendet für[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) und[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) nur Entitätseigenschaften und vereinfacht die Aufzählung.

### Beispiele

Wie man Eigenschaften auflistet mit **Entitätsfeld** Attribut:

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

### Siehe auch

* namensraum [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* Montage [Aspose.Tasks](../../)


