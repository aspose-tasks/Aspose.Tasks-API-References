---
title: "GanttBarStyle.Name"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttBarStyle. Obtiene o establece el nombre del estilo"
type: docs
weight: 150
url: /es/net/aspose.tasks.visualization/ganttbarstyle/name/
---
## GanttBarStyle.Name property

Obtiene o establece el nombre del estilo.

```csharp
public string Name { get; set; }
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


