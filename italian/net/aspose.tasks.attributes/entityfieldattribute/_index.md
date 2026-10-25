---
title: "Classe EntityFieldAttribute"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Attributes.EntityFieldAttribute. Rappresenta un attributo per le proprietà dell'entità"
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
| [EntityFieldAttribute](entityfieldattribute/)() | Il costruttore predefinito. |

## Osservazioni

Attributo utilizzato solo per le proprietà dell'entità [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) e [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), e semplifica la sua enumerazione.

## Esempi

Come enumerare le proprietà utilizzando l'attributo **EntityField**:

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

### Vedi anche

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


