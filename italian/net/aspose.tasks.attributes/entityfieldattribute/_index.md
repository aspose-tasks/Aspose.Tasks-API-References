---
title: Class EntityFieldAttribute
second_title: Riferimento all'API di Aspose.Tasks per .NET
description: Aspose.Tasks.Attributes.EntityFieldAttribute classe. Rappresenta un attributo per le proprietà dellentità.
type: docs
weight: 70
url: /it/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Rappresenta un attributo per le proprietà dell'entità.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | Default_Costruttore |

### Osservazioni

Attributo utilizzato per[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) e[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) solo proprietà dell'entità e ne semplifica l'enumerazione.

### Esempi

Come enumerare le proprietà utilizzando **EntityField** attributo:

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

### Guarda anche

* spazio dei nomi [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assemblea [Aspose.Tasks](../../)


