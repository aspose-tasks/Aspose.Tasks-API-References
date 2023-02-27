---
title: Class EntityFieldAttribute
second_title: Referencia de Aspose.Tasks para la API de .NET
description: Aspose.Tasks.Attributes.EntityFieldAttribute clase. Representa un atributo para las propiedades de la entidad.
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
| [EntityFieldAttribute](entityfieldattribute/)() | Constructor predeterminado |

### Observaciones

Atributo utilizado para[`Task`](../../aspose.tasks/task/) ,[`Resource`](../../aspose.tasks/resource/) ,[`Project`](../../aspose.tasks/project/) y[`ResourceAssignment`](../../aspose.tasks/resourceassignment/) propiedades de entidad solamente, y simplifica su enumeración.

### Ejemplos

Cómo enumerar propiedades usando **EntityField** atributo:

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

* espacio de nombres [Aspose.Tasks.Attributes](../../aspose.tasks.attributes/)
* asamblea [Aspose.Tasks](../../)


