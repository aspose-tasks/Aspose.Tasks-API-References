---
title: "TableField.WrapHeader"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TableField. Obtiene o establece un valor que indica si el encabezado de la columna de la tabla puede ajustarse a varias líneas o si debe truncarse cuando supera el ancho de la columna"
type: docs
weight: 70
url: /es/net/aspose.tasks/tablefield/wrapheader/
---
## TableField.WrapHeader property

Obtiene o establece un valor que indica si el encabezado de la columna de la tabla puede ajustarse a varias líneas, o si debe truncarse cuando supera el ancho de la columna.

```csharp
public bool WrapHeader { get; set; }
```

## Ejemplos

Muestra cómo leer las tablas del proyecto.

```csharp
var project = new Project(DataDir + "ReadTableData.mpp");

// obtener la tabla
var table = project.Tables.ToList()[0];
Console.WriteLine("Print table fields of {0}", table.Name);
Console.WriteLine("Table Fields Count" + table.TableFields.Count);

// mostrar la información de todos los campos de la tabla
foreach (var field in table.TableFields)
{
    Console.WriteLine("  Field: " + field.Field);
    Console.WriteLine("  Width: " + field.Width);
    Console.WriteLine("  Title: " + field.Title);
    Console.WriteLine("  Title Alignment: " + field.AlignTitle);
    Console.WriteLine("  Data Alignment: " + field.AlignData);
    Console.WriteLine("  Wrap Header: " + field.WrapHeader);
    Console.WriteLine("  Wrap Text: " + field.WrapText);
    Console.WriteLine();
}
```

### Ver también

* class [TableField](../)
* namespace [Aspose.Tasks](../../tablefield/)
* assembly [Aspose.Tasks](../../../)


