---
title: "Clase ResourceViewColumn"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.ResourceViewColumn. Clase de vista de proyectos utilizada en la vista ResourceUsage y la vista ResourceSheet"
type: docs
weight: 3350
url: /es/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Clase de vista del proyecto usada en la vista ResourceUsage y la vista ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Inicializa una nueva instancia de la clase `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Inicializa una nueva instancia de la clase `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Inicializa una nueva instancia de la clase `ResourceViewColumn`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Campo de columna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Obtiene el nombre de la columna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Obtiene o establece la alineación del texto (puede ser uno de los valores de la enumeración [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Obtiene o establece la devolución de llamada que puede usarse para personalizar la apariencia de las celdas de la columna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Obtiene el ancho de la columna. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Convierte el recurso actual al texto de la columna. |

## Ejemplos

Muestra cómo agregar columnas de vista de recursos para exportar.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// iterar sobre columnas
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Ver también

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


