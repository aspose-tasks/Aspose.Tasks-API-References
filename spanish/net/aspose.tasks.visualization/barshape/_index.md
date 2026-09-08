---
title: "Enumeración BarShape"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Aspose.Tasks.Visualization.BarShape enum. Forma de un rectángulo de barra"
type: docs
weight: 2950
url: /es/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Forma del rectángulo de una barra.

```csharp
public enum BarShape
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Full | `0` | Indica forma de barra rectangular completa. |
| HalfHeight | `1` | Indica forma de barra rectangular de media altura alineada en la parte superior. |
| HalfHeightBottom | `2` | Indica forma de barra rectangular de media altura alineada en la parte inferior. |
| Thin | `3` | Indica forma de línea alineada al centro. |
| None | `4` | Indica forma de barra Ninguna. |
| Middle | `5` | Indica forma de línea alineada al centro. |
| LineBottom | `6` | Indica forma de línea alineada en la parte inferior. |
| LineTop | `7` | Indica forma de línea alineada en la parte superior. |

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


