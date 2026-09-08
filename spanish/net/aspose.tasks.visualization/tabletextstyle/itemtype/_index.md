---
title: "TableTextStyle.ItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad TableTextStyle. Devuelve un valor del enum TextItemType."
type: docs
weight: 30
url: /es/net/aspose.tasks.visualization/tabletextstyle/itemtype/
---
## TableTextStyle.ItemType property

Devuelve un valor del enum [`TextItemType`](../../textitemtype/).

```csharp
public override TextItemType ItemType { get; }
```

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

* enum [TextItemType](../../textitemtype/)
* class [TableTextStyle](../)
* namespace [Aspose.Tasks.Visualization](../../tabletextstyle/)
* assembly [Aspose.Tasks](../../../)


