---
title: "Clase EntityFieldAttribute"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Attributes.EntityFieldAttribute. Representa un atributo para propiedades de entidad"
type: docs
weight: 70
url: /es/net/aspose.tasks.attributes/entityfieldattribute/
---
## EntityFieldAttribute class

Representa un atributo para las propiedades de la entidad.

```csharp
[AttributeUsage(AttributeTargets.Property)]
public class EntityFieldAttribute : Attribute
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [EntityFieldAttribute](entityfieldattribute/)() | El constructor predeterminado. |

## Observaciones

Atributo usado solo para propiedades de entidad de [`Task`](../../aspose.tasks/task/), [`Resource`](../../aspose.tasks/resource/), [`Project`](../../aspose.tasks/project/) y [`ResourceAssignment`](../../aspose.tasks/resourceassignment/), y simplifica su enumeración.

## Ejemplos

Cómo enumerar propiedades usando el atributo **EntityField**:

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

### Ver también

* namespace [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* assembly [Aspose.Tasks](../../)


