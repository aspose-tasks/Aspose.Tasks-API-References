---
title: "BarStyle.ItemType"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad BarStyle. Obtiene o establece BarItemType del estilo de barra"
type: docs
weight: 120
url: /es/net/aspose.tasks.visualization/barstyle/itemtype/
---
## BarStyle.ItemType property

Obtiene o establece [`BarItemType`](../../baritemtype/) del estilo de barra.

```csharp
public BarItemType ItemType { get; set; }
```

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

* enum [BarItemType](../../baritemtype/)
* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


