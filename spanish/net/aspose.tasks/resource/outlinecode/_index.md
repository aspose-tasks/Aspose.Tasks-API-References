---
title: "Resource.OutlineCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Resource. Obtiene un objeto OutlineCodeCollection. El valor de un código de esquema"
type: docs
weight: 540
url: /es/net/aspose.tasks/resource/outlinecode/
---
## Resource.OutlineCode property

Obtiene un objeto OutlineCodeCollection. El valor de un código de esquema.

```csharp
public OutlineCodeCollection OutlineCode { get; }
```

## Observaciones

Se requieren dos piezas de datos: un puntero a la tabla de códigos de esquema que se especifica mediante FieldID, y el valor que se especifica ya sea mediante ValueID o mediante el puntero ValueGUID a la lista de valores.

## Ejemplos

Muestra cómo trabajar con los valores de esquema de recurso.

```csharp
var project = new Project(DataDir + "OutlineCodes2003.mpp");

var res = project.Resources.GetById(2);
Assert.AreEqual(2, res.OutlineCode.Count);
foreach (var code in res.OutlineCode)
{
    object val = null;
    foreach (var def in project.OutlineCodes)
    {
        if (def.FieldId != code.FieldId)
        {
            continue;
        }

        foreach (var value in def.Values)
        {
            if (value.ValueId != code.ValueId)
            {
                continue;
            }

            val = value.Value;
            break;
        }
    }

    Console.WriteLine(val.ToString());
}
```

### Ver también

* class [OutlineCodeCollection](../../outlinecodecollection/)
* class [Resource](../)
* namespace [Aspose.Tasks](../../resource/)
* assembly [Aspose.Tasks](../../../)


