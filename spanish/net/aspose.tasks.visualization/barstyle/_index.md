---
title: "Clase BarStyle"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.BarStyle class. Cambia el estilo visual de la barra para el elemento en la vista del proyecto."
type: docs
weight: 2960
url: /es/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Cambiar el estilo visual de la barra para el elemento en la vista del proyecto.

```csharp
public class BarStyle
```

## Constructores

| Nombre | Descripción |
| --- | --- |
| [BarStyle](barstyle/)() | Inicializa una nueva instancia de la clase `BarStyle`. |

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Obtiene o establece el Color del estilo de barra. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Obtiene o establece [`BarShape`](./barshape/) del estilo de barra. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza en la parte inferior de la barra de la tarea. Sobrescribe el valor de la propiedad [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Obtiene o establece un campo que se mostrará en la parte inferior de la barra. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Obtiene o establece [`Shape`](../shape/) al final de la barra. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Obtiene o establece el Color de la forma al final de la barra. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Obtiene o establece el tipo de la forma final. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Obtiene o establece la posición del punto de inicio de la barra de gantt. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza dentro de la barra de la tarea. Sobrescribe el valor de la propiedad [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Obtiene o establece un campo que se mostrará dentro de la barra. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Obtiene o establece [`BarItemType`](../baritemtype/) del estilo de barra. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Obtiene o establece un convertidor definido por el usuario para obtener el texto que se renderiza a la izquierda de la barra de la tarea. Anula el valor de la propiedad [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Obtiene o establece un campo que se mostrará a la izquierda de la barra. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza a la derecha de la barra de la tarea. Sobrescribe el valor de la propiedad [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Obtiene o establece un campo que se mostrará a la derecha de la barra. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Obtiene o establece [`Shape`](../shape/) al comienzo de la barra. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Obtiene o establece el color de la forma al comienzo de la barra. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Obtiene o establece el tipo de la forma de inicio. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Obtiene o establece el estilo del texto de la barra. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Obtiene o establece la posición del punto de finalización de la barra de gantt. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Obtiene o establece el convertidor definido por el usuario para obtener el texto que se renderiza en la parte superior de la barra de la tarea. Sobrescribe el valor de la propiedad [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Obtiene o establece un campo que se mostrará en la parte superior de la barra. |

## Ejemplos

Muestra cómo usar estilos de barra personalizados.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// agrega un estilo de barra para tareas de hito
var style = new BarStyle();
// establece <see cref=\"T:Aspose.Tasks.Visualization.BarItemType\" /> del estilo de barra
style.ItemType = BarItemType.Milestone;
// establece <see cref=\"T:System.Drawing.Color\" /> del estilo de barra.
style.BarColor = Color.Green;
// establece <see cref=\"P:Aspose.Tasks.Visualization.BarStyle.BarShape\" /> del estilo de barra
style.BarShape = BarShape.HalfHeight;
// establecer <see cref="T:Aspose.Tasks.Visualization.Shape" /> al comienzo de la barra
style.StartShape = Shape.LeftBracket;
// establecer <see cref="T:System.Drawing.Color" /> del shape al comienzo de la barra
style.StartShapeColor = Color.Aqua;
// establecer <see cref="T:Aspose.Tasks.Visualization.Shape" /> al final de la barra
style.EndShape = Shape.RightBracket;
// establecer <see cref="T:System.Drawing.Color" /> del shape al final de la barra
style.EndShapeColor = Color.Aquamarine;
// conjunto del texto a renderizar a la derecha de la barra.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// existe una característica que permite convertir un texto de la barra
// establezcamos el convertidor para obtener el texto de la barra a renderizar.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// guardar el proyecto
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Ver también

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


