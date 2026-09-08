---
title: "Clase OutlineCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.OutlineCode. Representa un valor de un código de esquema"
type: docs
weight: 1150
url: /es/net/aspose.tasks/outlinecode/
---
## OutlineCode class

Representa un valor de un código de esquema.

```csharp
public class OutlineCode
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [OutlineCode](outlinecode/#constructor)() | Inicializa una nueva instancia de la clase `OutlineCode`. |
| [OutlineCode](outlinecode/#constructor_1)(OutlineCodeDefinition, OutlineValue) | Inicializa una nueva instancia de la clase `OutlineCode` usando el Código de esquema especificado y uno de sus valores. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [FieldId](../../aspose.tasks/outlinecode/fieldid/) { get; set; } | Obtiene o establece el valor numérico del campo personalizado Id del proyecto. |
| [ValueGuid](../../aspose.tasks/outlinecode/valueguid/) { get; set; } | Obtiene o establece el GUID del valor en la lista de valores. El ValueGuid coincide con el FieldGuid en la lista de valores. |
| [ValueId](../../aspose.tasks/outlinecode/valueid/) { get; set; } | Obtiene o establece el Id en la lista de valores asociado con la definición en la colección de códigos de esquema. |

## Observaciones

Se requieren dos piezas de datos: un puntero a la tabla de códigos de esquema que se especifica mediante el FieldId, y el valor que se especifica ya sea por el puntero ValueId o ValueGuid a la lista de valores.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


