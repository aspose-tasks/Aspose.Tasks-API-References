---
title: "Enumeración Shape"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Enumeración Aspose.Tasks.Visualization.Shape. Forma de un marcador al inicio o al final del estilo de barra que se renderiza al guardar datos de vista en algunos de SaveFileFormat"
type: docs
weight: 3360
url: /es/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Forma de un marcador al inicio o al final del estilo de barra que se renderiza al guardar datos de vista en algunos de [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Indica la forma None. |
| VerticalLine | `1` | Indica la forma Vertical line. |
| Pentagon | `2` | Indica la forma Pentagon. |
| Triangle | `3` | Indica la forma Triangle. |
| LeftBracket | `4` | Indica la forma Left bracket. |
| RightBracket | `5` | Indica la forma Right bracket. |
| ArrowDown | `6` | Indica la forma ArrowDown. |
| LeftFade | `7` | Indica la forma Left fade. |
| RightFade | `8` | Indica la forma Right fade. |
| Diamond | `9` | Indica la forma Diamond. |
| Circle | `10` | Indica la forma Circle. |

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


