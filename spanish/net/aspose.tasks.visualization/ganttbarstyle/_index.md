---
title: "Clase GanttBarStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.GanttBarStyle clase. Representa un estilo de barra utilizado por MSP en la vista de diagrama de Gantt"
type: docs
weight: 3070
url: /es/net/aspose.tasks.visualization/ganttbarstyle/
---
## GanttBarStyle class

Representa un estilo de barra usado por MSP en la vista de diagrama de Gantt.

```csharp
public class GanttBarStyle
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [GanttBarStyle](ganttbarstyle/)() | Inicializa una nueva instancia de la clase `GanttBarStyle`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BottomBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/bottombartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza en la parte inferior de la barra de la tarea. Sobrescribe el valor de la propiedad [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/ganttbarstyle/bottomfield/) { get; set; } | Obtiene o establece los datos que se mostrarán en la parte inferior de la barra. [`Field`](../../aspose.tasks/field/). |
| [EndShape](../../aspose.tasks.visualization/ganttbarstyle/endshape/) { get; set; } | Obtiene o establece la forma final de la barra. |
| [EndShapeColor](../../aspose.tasks.visualization/ganttbarstyle/endshapecolor/) { get; set; } | Obtiene o establece el color de la forma final. |
| [EndShapeType](../../aspose.tasks.visualization/ganttbarstyle/endshapetype/) { get; set; } | Obtiene o establece el tipo de la forma final. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/ganttbarstyle/from/) { get; set; } | Obtiene o establece la posición del punto de inicio de la barra de gantt. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/insidebartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza dentro de la barra de la tarea. Sobrescribe el valor de la propiedad [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/ganttbarstyle/insidefield/) { get; set; } | Obtiene o establece los datos que se mostrarán dentro de la barra. [`Field`](../../aspose.tasks/field/). |
| [LeftBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/leftbartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza a la izquierda de la barra de la tarea. Sobrescribe el valor de la propiedad [`LeftField`](./leftfield/). No se persiste en el formato MPP. |
| [LeftField](../../aspose.tasks.visualization/ganttbarstyle/leftfield/) { get; set; } | Obtiene o establece los datos que se mostrarán a la izquierda de la barra. [`Field`](../../aspose.tasks/field/). |
| [MiddleFillPattern](../../aspose.tasks.visualization/ganttbarstyle/middlefillpattern/) { get; set; } | Obtiene o establece un patrón de relleno de la barra de gantt. |
| [MiddleShape](../../aspose.tasks.visualization/ganttbarstyle/middleshape/) { get; set; } | Obtiene o establece una forma intermedia de la barra. |
| [MiddleShapeColor](../../aspose.tasks.visualization/ganttbarstyle/middleshapecolor/) { get; set; } | Obtiene o establece el color de la forma intermedia. |
| [Name](../../aspose.tasks.visualization/ganttbarstyle/name/) { get; set; } | Obtiene o establece el nombre del estilo. |
| [ParentStyle](../../aspose.tasks.visualization/ganttbarstyle/parentstyle/) { get; set; } | Obtiene o establece el estilo padre (o común) para el estilo personalizado específico de la tarea. |
| [RightBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/rightbartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza a la derecha de la barra de la tarea. Sobrescribe el valor de la propiedad [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/ganttbarstyle/rightfield/) { get; set; } | Obtiene o establece los datos que se mostrarán a la derecha de la barra. [`Field`](../../aspose.tasks/field/). |
| [Row](../../aspose.tasks.visualization/ganttbarstyle/row/) { get; set; } | Obtiene o establece un número de fila. Puede ser de 1 a 4 (1 es el valor predeterminado). |
| [ShowForCategories](../../aspose.tasks.visualization/ganttbarstyle/showforcategories/) { get; set; } | Obtiene o establece las categorías de tareas a las que se aplica el estilo. Es aplicable a los estilos padre (o comunes) de las barras en el diagrama de Gantt (ver [`BarStyles`](../../aspose.tasks/ganttchartview/barstyles/)). |
| [ShowForTaskUid](../../aspose.tasks.visualization/ganttbarstyle/showfortaskuid/) { get; set; } | Obtiene o establece el Id único de una tarea a la que se aplica el estilo. Es aplicable a los estilos específicos de tarea de las barras en el diagrama de Gantt (ver [`CustomBarStyles`](../../aspose.tasks/ganttchartview/custombarstyles/)). |
| [StartShape](../../aspose.tasks.visualization/ganttbarstyle/startshape/) { get; set; } | Obtiene o establece la forma de inicio de la barra. |
| [StartShapeColor](../../aspose.tasks.visualization/ganttbarstyle/startshapecolor/) { get; set; } | Obtiene o establece el color de la forma de inicio. |
| [StartShapeType](../../aspose.tasks.visualization/ganttbarstyle/startshapetype/) { get; set; } | Obtiene o establece el tipo de la forma de inicio. |
| [To](../../aspose.tasks.visualization/ganttbarstyle/to/) { get; set; } | Obtiene o establece la posición del punto de finalización de la barra de gantt. |
| [TopBarTextConverter](../../aspose.tasks.visualization/ganttbarstyle/topbartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza en la parte superior de la barra de la tarea. Sobrescribe el valor de la propiedad [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/ganttbarstyle/topfield/) { get; set; } | Obtiene o establece los datos que se mostrarán en la parte superior de la barra. |

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

Muestra cómo leer los estilos de barra personalizados de una vista.

```csharp
var project = new Project(DataDir + "CustomBarStyle.mpp");

var view = (GanttChartView)project.DefaultView;
Console.WriteLine("Custom bar styles count: {0}", view.CustomBarStyles.Count);

var style1 = view.CustomBarStyles[0];
Console.WriteLine("Style1.ParentStyle Name: {0}", style1.ParentStyle.Name);
Console.WriteLine("Style1.LeftField: {0}", style1.LeftField);
Console.WriteLine("Style1.RightField: {0}", style1.RightField);
Console.WriteLine("Style1.TopField: {0}", style1.TopField);
Console.WriteLine("Style1.BottomField: {0}", style1.BottomField);
Console.WriteLine("Style1.InsideField: {0}", style1.InsideField);
Console.WriteLine("Style1.From: {0}", style1.From);
Console.WriteLine("Style1.To: {0}", style1.To);
Console.WriteLine("Style1.Row: {0}", style1.Row);

var style2 = view.CustomBarStyles[1];
Console.WriteLine("Style2.LeftField: {0}", style2.LeftField);
Console.WriteLine("Style2.RightField: {0}", style2.RightField);
Console.WriteLine("Style2.TopField: {0}", style2.TopField);
Console.WriteLine("Style2.BottomField: {0}", style2.BottomField);
Console.WriteLine("Style2.InsideField: {0}", style2.InsideField);
Console.WriteLine("Style2.From: {0}", style2.From);
Console.WriteLine("Style2.To: {0}", style2.To);
Console.WriteLine("Style2.Row: {0}", style1.Row);

var style3 = view.CustomBarStyles[2];
Console.WriteLine("Style3.LeftField: {0}", style3.LeftField);
Console.WriteLine("Style3.RightField: {0}", style3.RightField);
Console.WriteLine("Style3.TopField: {0}", style3.TopField);
Console.WriteLine("Style3.BottomField: {0}", style3.BottomField);
Console.WriteLine("Style3.InsideField: {0}", style3.InsideField);

Console.WriteLine("Style3.StartShape: {0}", style3.StartShape);
Console.WriteLine("Style3.StartShapeType: {0}", style3.StartShapeType);
Console.WriteLine("Style3.StartShapeColor: {0}", style3.StartShapeColor);

Console.WriteLine("Style3.EndShape: {0}", style3.EndShape);
Console.WriteLine("Style3.EndShapeType: {0}", style3.EndShapeType);
Console.WriteLine("Style3.EndShapeColor: {0}", style3.EndShapeColor);

Console.WriteLine("Style3.MiddleShape: {0}", style3.MiddleShape);
Console.WriteLine("Style3.MiddleFillPattern: {0}", style3.MiddleFillPattern);
Console.WriteLine("Style3.MiddleShapeColor: {0}", style3.MiddleShapeColor);
Console.WriteLine("Style3.From: {0}", style3.From);
Console.WriteLine("Style3.To: {0}", style3.To);
Console.WriteLine("Style3.Row: {0}", style1.Row);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


