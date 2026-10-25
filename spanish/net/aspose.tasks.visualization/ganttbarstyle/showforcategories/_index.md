---
title: "GanttBarStyle.ShowForCategories"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttBarStyle. Obtiene o establece las categorías de tarea para las que se aplica el estilo. Es aplicable a los estilos padre o comunes de las barras en el diagrama de Gantt, vea BarStyles"
type: docs
weight: 200
url: /es/net/aspose.tasks.visualization/ganttbarstyle/showforcategories/
---
## GanttBarStyle.ShowForCategories property

Obtiene o establece las categorías de tarea para las que se aplica el estilo. Es aplicable a los estilos padre (o comunes) de las barras en el diagrama de Gantt (ver [`BarStyles`](../../../aspose.tasks/ganttchartview/barstyles/)).

```csharp
public IList<GanttBarShowFor> ShowForCategories { get; set; }
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

* enum [GanttBarShowFor](../../ganttbarshowfor/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


