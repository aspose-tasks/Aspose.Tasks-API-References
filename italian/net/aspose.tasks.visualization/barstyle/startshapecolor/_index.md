---
title: "BarStyle.StartShapeColor"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "BarStyle proprietà. Ottiene o imposta il colore della forma all'inizio della barra"
type: docs
weight: 180
url: /it/net/aspose.tasks.visualization/barstyle/startshapecolor/
---
## BarStyle.StartShapeColor property

Ottiene o imposta il colore della forma all'inizio della barra.

```csharp
public Color StartShapeColor { get; set; }
```

## Esempi

Mostra come utilizzare stili di barra personalizzati.

```csharp
var project = new Project(DataDir + "Project2.mpp");
SaveOptions options = new PdfSaveOptions
{
    BarStyles = new List<BarStyle>()
};

// aggiungi uno stile di barra per attività milestone
var style = new BarStyle();
// imposta <see cref="T:Aspose.Tasks.Visualization.BarItemType" /> dello stile della barra
style.ItemType = BarItemType.Milestone;
// imposta <see cref="T:System.Drawing.Color" /> dello stile della barra.
style.BarColor = Color.Green;
// imposta <see cref="P:Aspose.Tasks.Visualization.BarStyle.BarShape" /> dello stile della barra
style.BarShape = BarShape.HalfHeight;
// set <see cref="T:Aspose.Tasks.Visualization.Shape" /> all'inizio della barra
style.StartShape = Shape.LeftBracket;
// imposta <see cref="T:System.Drawing.Color" /> della forma all'inizio della barra
style.StartShapeColor = Color.Aqua;
// imposta <see cref="T:Aspose.Tasks.Visualization.Shape" /> alla fine della barra
style.EndShape = Shape.RightBracket;
// imposta <see cref="T:System.Drawing.Color" /> della forma alla fine della barra
style.EndShapeColor = Color.Aquamarine;
// imposta il testo da visualizzare a destra della barra.
style.TextStyle = new TextStyle();
style.TextStyle.BackgroundColor = Color.Black;

// esiste una funzionalità che consente di convertire il testo della barra
// impostiamo il convertitore per ottenere il testo da visualizzare sulla barra.
style.LeftBarTextConverter = task =>
{
    if (!task.Get(Tsk.Name).StartsWith("T"))
    {
        task.Set(Tsk.Name, "T" + task.Get(Tsk.Name));
    }

    return task.Get(Tsk.Name);
};

options.BarStyles.Add(style);

// salva il progetto
project.Save(OutDir + "WorkWithBarStyle_out.mpp", options);
```

### Vedi anche

* class [BarStyle](../)
* namespace [Aspose.Tasks.Visualization](../../barstyle/)
* assembly [Aspose.Tasks](../../../)


