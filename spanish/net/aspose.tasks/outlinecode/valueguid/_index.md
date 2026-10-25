---
title: "OutlineCode.ValueGuid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad de OutlineCode. Obtiene o establece el GUID del valor en la lista de valores. El ValueGuid coincide con el FieldGuid en la lista de valores"
type: docs
weight: 30
url: /es/net/aspose.tasks/outlinecode/valueguid/
---
## OutlineCode.ValueGuid property

Obtiene o establece el GUID del valor en la lista de valores. El ValueGuid coincide con el FieldGuid en la lista de valores.

```csharp
public string ValueGuid { get; set; }
```

## Ejemplos

Muestra cómo leer los códigos de esquema de la tarea.

```csharp
var project = new Project(DataDir + "OutlineValues2010.mpp");

// leer códigos de esquema
foreach (var task in project.RootTask.SelectAllChildTasks())
{
    if (task.OutlineCodes.Count <= 0)
    {
        continue;
    }

    Console.WriteLine("Print outline codes of the task: " + task.Get(Tsk.Name));
    foreach (var value in task.OutlineCodes)
    {
        Console.WriteLine("  Field Id: " + value.FieldId);
        Console.WriteLine("  Value Guid: " + value.ValueGuid);
        Console.WriteLine("  Value Id: " + value.ValueId);
    }
}
```

### Ver también

* class [OutlineCode](../)
* namespace [Aspose.Tasks](../../outlinecode/)
* assembly [Aspose.Tasks](../../../)


