---
title: "GanttBarStyle.ShowForTaskUid"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttBarStyle. Obtiene o establece el Id único de una tarea para la cual se aplica el estilo. Es aplicable a estilos específicos de tarea de las barras en el diagrama de Gantt, ver CustomBarStyles"
type: docs
weight: 210
url: /es/net/aspose.tasks.visualization/ganttbarstyle/showfortaskuid/
---
## GanttBarStyle.ShowForTaskUid property

Obtiene o establece el Id único de una tarea para la cual se aplica el estilo. Es aplicable a estilos específicos de tarea de las barras en el diagrama de Gantt (ver [`CustomBarStyles`](../../../aspose.tasks/ganttchartview/custombarstyles/)).

```csharp
public int? ShowForTaskUid { get; set; }
```

## Ejemplos

Muestra cómo usar las categorías ShowFor.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var view = (GanttChartView)project.DefaultView;

var barStyle = this.GetCustomBarStyle();
barStyle.ShowForTaskUid = null;

var showForCategories = new[]
{
    GanttBarShowFor.Active,
    GanttBarShowFor.NotSummary,
    GanttBarShowFor.Milestone,
    GanttBarShowFor.Finished
};

barStyle.ShowForCategories = new List<GanttBarShowFor>(showForCategories);
barStyle.Name = "My common style";
view.BarStyles.Add(barStyle);

// trabajar con el proyecto...
```

### Ver también

* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


