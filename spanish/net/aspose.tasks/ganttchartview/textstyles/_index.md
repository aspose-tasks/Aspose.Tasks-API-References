---
title: "GanttChartView.TextStyles"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttChartView. Obtiene o establece una lista de TextStyle de la vista de diagrama de Gantt"
type: docs
weight: 170
url: /es/net/aspose.tasks/ganttchartview/textstyles/
---
## GanttChartView.TextStyles property

Obtiene o establece una lista de [`TextStyle`](../../../aspose.tasks.visualization/textstyle/) de la vista de diagrama de Gantt.

```csharp
public List<TextStyle> TextStyles { get; set; }
```

## Ejemplos

Muestra cómo leer los estilos de texto del diagrama de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[0];

// iterar sobre los estilos de texto de la vista del diagrama de Gantt
foreach (var style in view.TextStyles)
{
    Console.WriteLine("Style Item Type: " + style.ItemType);
    Console.WriteLine("Style Font name: " + style.Font.FontFamily);
    Console.WriteLine();
}
```

### Ver también

* class [TextStyle](../../../aspose.tasks.visualization/textstyle/)
* class [GanttChartView](../)
* namespace [Aspose.Tasks](../../ganttchartview/)
* assembly [Aspose.Tasks](../../../)


