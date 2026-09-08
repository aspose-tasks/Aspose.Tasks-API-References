---
title: "GanttBarStyle.LeftBarTextConverter"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad GanttBarStyle. Obtiene o establece un convertidor definido por el usuario para obtener el texto que se mostrará en el lado izquierdo de la barra de tareas. Sobrescribe el valor de la propiedad LeftField. No se persiste en el formato MPP"
type: docs
weight: 100
url: /es/net/aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/
---
## GanttBarStyle.LeftBarTextConverter property

Obtiene o establece un convertidor definido por el usuario para obtener el texto que se mostrará en el lado izquierdo de la barra de la tarea. Sobrescribe el valor de la propiedad [`LeftField`](../leftfield/). No se persiste en el formato MPP.

```csharp
public TaskBarTextConverter LeftBarTextConverter { get; set; }
```

## Ejemplos

Muestra cómo usar estilos de barra personalizados en la vista del diagrama de Gantt.

```csharp
var project = new Project(DataDir + "Project2.mpp");

var ganttChartView = (GanttChartView)project.Views.First(v => v.Name == "Gantt &Chart");
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Timescale = Timescale.DefinedInView;
saveOptions.ViewSettings = ganttChartView;

// Los estilos de barra pueden ser específicos de tarea (ubicados en GanttChartView.CustomBarStyles).
// o específicos de categoría (ubicados en GanttChartView.BarStyles).
foreach (GanttBarStyle ganttBarStyle in ganttChartView.CustomBarStyles)
{
    if (ganttBarStyle.ShowForTaskUid != 4)
    {
        continue;
    }

    // Para fines de demostración, estamos modificando el estilo de la tarea con ID único = 4.
    // Aquí establecemos el campo (TaskName) para que se muestre a la izquierda de la barra de la tarea.
    ganttBarStyle.LeftField = Field.TaskName;
    // Aquí establecemos un convertidor personalizado para controlar qué texto se debe renderizar dentro de la barra de la tarea.
    ganttBarStyle.InsideBarTextConverter = task => "Hours rem.: " + (int)task.Get(Tsk.RemainingWork).TimeSpan.TotalHours;

    ganttBarStyle.MiddleShapeColor = Color.Green;
    ganttBarStyle.MiddleShape = GanttBarMiddleShape.LineTop;
    ganttBarStyle.StartShape = GanttBarEndShape.LeftBracket;
    ganttBarStyle.StartShapeColor = Color.Aqua;
    ganttBarStyle.EndShape = GanttBarEndShape.RightBracket;
    ganttBarStyle.EndShapeColor = Color.Aquamarine;
}

foreach (GanttBarStyle ganttBarStyle in ganttChartView.BarStyles)
{
    if (!ganttBarStyle.ShowForCategories.Contains(GanttBarShowFor.Milestone))
    {
        continue;
    }

    // Para fines de demostración, estamos modificando los estilos aplicables a tareas de hito.

    ganttBarStyle.StartShape = GanttBarEndShape.Diamond;
    ganttBarStyle.RightField = Field.TaskActualFinish;
    ganttBarStyle.TopBarTextConverter = task => task.Get(Tsk.ActualStart).Day.ToString();
}

project.Save(OutDir + "WorkWithGanttChartViewBarStyles_out.pdf", saveOptions);
```

### Ver también

* delegate [TaskBarTextConverter](../../taskbartextconverter/)
* class [GanttBarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../ganttbarstyle/)
* assembly [Aspose.Tasks](../../../)


