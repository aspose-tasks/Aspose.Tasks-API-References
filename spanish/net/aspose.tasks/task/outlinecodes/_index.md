---
title: "Task.OutlineCodes"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Task. Obtiene o establece un objeto OutlineCodeCollection"
type: docs
weight: 880
url: /es/net/aspose.tasks/task/outlinecodes/
---
## Task.OutlineCodes property

Obtiene o establece el objeto [`OutlineCodeCollection`](../../outlinecodecollection/).

```csharp
public OutlineCodeCollection OutlineCodes { get; set; }
```

## Observaciones

Se requieren dos piezas de datos: un puntero a la tabla de códigos de esquema que se especifica mediante FieldID, y el valor que se especifica ya sea mediante ValueID o mediante el puntero ValueGUID a la lista de valores.

## Ejemplos

Muestra cómo leer los valores de código de esquema de la tarea.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");
    var mapping = new Dictionary<string, OutlineValueCollection>();

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var code in project.OutlineCodes)
    {
        mapping.Add(code.FieldId, code.Values);
    }

    var task = project.RootTask.Children.GetById(2);
    foreach (var code in task.OutlineCodes)
    {
        var val = GetOutlineValue(mapping[code.FieldId], code.ValueId);
        Console.WriteLine("Outline value: " + val);
    }
}

public static object GetOutlineValue(OutlineValueCollection collection, int valueId)
{
    object obj = null;

    // ReSharper disable once LoopCanBeConvertedToQuery //ExSkip
    foreach (var value in collection)
    {
        if (value.ValueId != valueId)
        {
            continue;
        }

        obj = value.Value;
        break;
    }

    return obj;
}
```

### Ver también

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


