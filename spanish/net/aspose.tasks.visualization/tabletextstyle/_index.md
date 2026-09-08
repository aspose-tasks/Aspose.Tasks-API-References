---
title: "Clase TableTextStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Clase Aspose.Tasks.Visualization.TableTextStyle. Representa un estilo de texto en una tabla de vista"
type: docs
weight: 3370
url: /es/net/aspose.tasks.visualization/tabletextstyle/
---
## TableTextStyle class

Representa un estilo de texto en una tabla de vista.

```csharp
public class TableTextStyle : TextStyle
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [TableTextStyle](tabletextstyle/#constructor)(int) | Inicializa una nueva instancia de la clase `TableTextStyle`. |
| [TableTextStyle](tabletextstyle/#constructor_1)(int, FontDescriptor) | Inicializa una nueva instancia de la clase `TableTextStyle` con la fuente especificada. |
| [TableTextStyle](tabletextstyle/#constructor_2)(int, FontStyles) | Inicializa una nueva instancia de la clase `TableTextStyle` con la configuración de fuente predeterminada y el estilo de fuente especificado. |
| [TableTextStyle](tabletextstyle/#constructor_3)(int, float, FontStyles) | Inicializa una nueva instancia de la clase `TableTextStyle` con el tamaño de fuente y el estilo de fuente especificados. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BackgroundColor](../../aspose.tasks.visualization/textstyle/backgroundcolor/) { get; set; } | Obtiene o establece el color de fondo del estilo de texto. [`Color`](../textstyle/color/). |
| [BackgroundPattern](../../aspose.tasks.visualization/textstyle/backgroundpattern/) { get; set; } | Obtiene o establece el patrón de fondo del estilo de texto. [`BackgroundPattern`](../textstyle/backgroundpattern/). |
| [Color](../../aspose.tasks.visualization/textstyle/color/) { get; set; } | Obtiene o establece el color del texto. |
| [Field](../../aspose.tasks.visualization/tabletextstyle/field/) { get; set; } | Obtiene o establece un campo al que se aplicará el estilo. [`Field`](./field/). |
| [Font](../../aspose.tasks.visualization/textstyle/font/) { get; set; } | Obtiene o establece la fuente del estilo de texto. |
| override [ItemType](../../aspose.tasks.visualization/tabletextstyle/itemtype/) { get; } | Devuelve un valor del enumerado [`TextItemType`](../textitemtype/). |
| [RowUid](../../aspose.tasks.visualization/tabletextstyle/rowuid/) { get; } | Obtiene un id único de fila. Devuelve -1 si el estilo se aplicará a todas las filas de una vista. |

## Ejemplos

Muestra cómo personalizar los estilos de texto de tabla que se utilizan para dar estilo a diferentes elementos de texto en un proyecto.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.NewTasksAreManual, false);

var view = (GanttChartView)project.Views.ToList()[0];

// establecer estilo de texto del nombre de la primera tarea
var style1 = new TableTextStyle(1);
// establecer un campo al que se aplicará el estilo.
style1.Field = Field.TaskName;
// establecer <see cref=\"P:Aspose.Tasks.Visualization.TextStyle.Font\" /> del estilo de texto.
style1.Font = new FontDescriptor("Impact", 12F, FontStyles.Bold | FontStyles.Italic);
// establecer el tamaño en puntos de la fuente del estilo de texto.

// establecer estilo de texto de la duración de la segunda tarea
var style2 = new TableTextStyle(2);
style2.Field = Field.TaskDurationText;
style2.Font = new FontDescriptor("Impact", 16F, FontStyles.Underline);

view.TableTextStyles.Add(style1);
view.TableTextStyles.Add(style2);

SimpleSaveOptions options = new MPPSaveOptions
{
    // establecer una bandera que indique que los datos de vista deben escribirse
    WriteViewData = true
};
project.Save(OutDir + "WorkWithTableTextStyle_out.mpp", options);
```

### Ver también

* class [TextStyle](../textstyle/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


