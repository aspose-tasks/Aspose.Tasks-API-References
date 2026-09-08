---
title: "Project.Tables"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad Project. Obtiene una lista de objetos Table"
type: docs
weight: 900
url: /es/net/aspose.tasks/project/tables/
---
## Project.Tables property

Obtiene una lista de objetos [`Table`](../../table/).

```csharp
public TableCollection Tables { get; }
```

## Ejemplos

Muestra cómo configurar las propiedades de Gantt Chart.

```csharp
var project = new Project(DataDir + "Project5.mpp");
    var task = project.RootTask.Children.Add("New Activity");

    // Definir nuevo atributo personalizado
    var definition = ExtendedAttributeDefinition.CreateTaskDefinition(ExtendedAttributeTask.Text1, null);
    project.ExtendedAttributes.Add(definition);

    // Agregar atributo de texto personalizado a la tarea creada.
    task.ExtendedAttributes.Add(definition.CreateExtendedAttribute("Activity attribute"));

    // Personaliza la tabla añadiendo un campo de atributo de texto
    var field = new TableField
    {
        Field = Field.TaskText1,
        Width = 20,
        Title = "Custom attribute",
        AlignTitle = HorizontalStringAlignment.Center,
        AlignData = HorizontalStringAlignment.Center
    };

    var table = project.Tables.ToList()[0];
    table.TableFields.Insert(3, field);

    project.Save(OutDir + @"ConfigureGantChart_out.mpp", new MPPSaveOptions { WriteViewData = true });
}
catch (NotSupportedException ex)
{
    Console.WriteLine(
        ex.Message
        + "\nThis example will only work if you apply a valid Aspose License. You can purchase full license or get 30 day temporary license from http:// Www.aspose.com/purchase/default.aspx.");
}
```

### Ver también

* class [TableCollection](../../tablecollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


