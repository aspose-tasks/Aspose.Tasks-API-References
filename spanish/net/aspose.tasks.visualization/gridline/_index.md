---
title: "Clase Gridline"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.Gridline. La línea horizontal o vertical que aparece en la vista del proyecto"
type: docs
weight: 3100
url: /es/net/aspose.tasks.visualization/gridline/
---
## Gridline class

La línea horizontal o vertical que aparece en la vista del proyecto.

```csharp
public class Gridline
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [Gridline](gridline/)() | Inicializa una nueva instancia de la clase `Gridline`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [Color](../../aspose.tasks.visualization/gridline/color/) { get; set; } | Obtiene o establece el [`Color`](./color/) de una línea de cuadrícula. |
| [GridlineType](../../aspose.tasks.visualization/gridline/gridlinetype/) { get; set; } | Obtiene o establece el tipo de línea de cuadrícula ([`GridlineType`](./gridlinetype/)). |
| [Pattern](../../aspose.tasks.visualization/gridline/pattern/) { get; set; } | Obtiene o establece el [`LinePattern`](../linepattern/) de una línea de cuadrícula. |

## Métodos

| Nombre | Descripción |
| --- | --- |
| override [Equals](../../aspose.tasks.visualization/gridline/equals/)(object) | Devuelve una bandera que indica si esta instancia es igual al objeto especificado. |
| override [GetHashCode](../../aspose.tasks.visualization/gridline/gethashcode/)() | Devuelve un valor de código hash para la instancia de la clase `Gridline`. |

## Ejemplos

Muestra cómo trabajar con líneas de cuadrícula al guardar en formatos visuales.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");
var options = new ImageSaveOptions(SaveFileFormat.Png);

var gridline = new Gridline
{
    // establece el tipo de línea de cuadrícula (<see cref=\"P:Aspose.Tasks.Visualization.Gridline.GridlineType\" />).
    GridlineType = GridlineType.GanttRow, 
    // establece el <see cref=\"T:Aspose.Tasks.Visualization.LinePattern\" /> de una línea de cuadrícula
    Pattern = LinePattern.Dashed
};

options.Gridlines = new List<Gridline>();
options.Gridlines.Add(gridline);

project.Save(OutDir + "PrintProjectPagesToSeparateFiles_out.png", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


