---
title: "Class BarStyle"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.BarStyle. Modifica lo stile visivo della barra per l'elemento nella visualizzazione del progetto."
type: docs
weight: 2960
url: /it/net/aspose.tasks.visualization/barstyle/
---
## BarStyle class

Modifica lo stile visivo della barra per l'elemento nella visualizzazione del progetto.

```csharp
public class BarStyle
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [BarStyle](barstyle/)() | Inizializza una nuova istanza della classe `BarStyle`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [BarColor](../../aspose.tasks.visualization/barstyle/barcolor/) { get; set; } | Ottiene o imposta il colore dello stile della barra. |
| [BarShape](../../aspose.tasks.visualization/barstyle/barshape/) { get; set; } | Ottiene o imposta [`BarShape`](./barshape/) dello stile della barra. |
| [BottomBarTextConverter](../../aspose.tasks.visualization/barstyle/bottombartextconverter/) { get; set; } | Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare nella parte inferiore della barra dell'attività. Sovrascrive il valore della proprietà [`BottomField`](./bottomfield/). |
| [BottomField](../../aspose.tasks.visualization/barstyle/bottomfield/) { get; set; } | Ottiene o imposta un campo da visualizzare nella parte inferiore della barra. |
| [EndShape](../../aspose.tasks.visualization/barstyle/endshape/) { get; set; } | Ottiene o imposta [`Shape`](../shape/) alla fine della barra. |
| [EndShapeColor](../../aspose.tasks.visualization/barstyle/endshapecolor/) { get; set; } | Ottiene o imposta il colore della forma alla fine della barra. |
| [EndShapeType](../../aspose.tasks.visualization/barstyle/endshapetype/) { get; set; } | Ottiene o imposta il tipo della forma finale. [`GanttBarType`](../ganttbartype/). |
| [From](../../aspose.tasks.visualization/barstyle/from/) { get; set; } | Ottiene o imposta la posizione del punto di inizio della barra Gantt. [`Field`](../../aspose.tasks/field/). |
| [InsideBarTextConverter](../../aspose.tasks.visualization/barstyle/insidebartextconverter/) { get; set; } | Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare all'interno della barra dell'attività. Sovrascrive il valore della proprietà [`InsideField`](./insidefield/). |
| [InsideField](../../aspose.tasks.visualization/barstyle/insidefield/) { get; set; } | Ottiene o imposta un campo da visualizzare all'interno della barra. |
| [ItemType](../../aspose.tasks.visualization/barstyle/itemtype/) { get; set; } | Ottiene o imposta [`BarItemType`](../baritemtype/) dello stile della barra. |
| [LeftBarTextConverter](../../aspose.tasks.visualization/barstyle/leftbartextconverter/) { get; set; } | Ottiene o imposta un convertitore definito dall'utente per ottenere il testo da visualizzare a sinistra della barra dell'attività. Sovrascrive il valore della proprietà [`LeftField`](./leftfield/). |
| [LeftField](../../aspose.tasks.visualization/barstyle/leftfield/) { get; set; } | Ottiene o imposta un campo da visualizzare a sinistra della barra. |
| [RightBarTextConverter](../../aspose.tasks.visualization/barstyle/rightbartextconverter/) { get; set; } | Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare a destra della barra dell'attività. Sovrascrive il valore della proprietà [`RightField`](./rightfield/). |
| [RightField](../../aspose.tasks.visualization/barstyle/rightfield/) { get; set; } | Ottiene o imposta un campo da visualizzare a destra della barra. |
| [StartShape](../../aspose.tasks.visualization/barstyle/startshape/) { get; set; } | Ottiene o imposta [`Shape`](../shape/) all'inizio della barra. |
| [StartShapeColor](../../aspose.tasks.visualization/barstyle/startshapecolor/) { get; set; } | Ottiene o imposta il colore della forma all'inizio della barra. |
| [StartShapeType](../../aspose.tasks.visualization/barstyle/startshapetype/) { get; set; } | Ottiene o imposta il tipo della forma di inizio. |
| [TextStyle](../../aspose.tasks.visualization/barstyle/textstyle/) { get; set; } | Ottiene o imposta lo stile del testo della barra. |
| [To](../../aspose.tasks.visualization/barstyle/to/) { get; set; } | Ottiene o imposta la posizione del punto finale della barra Gantt. |
| [TopBarTextConverter](../../aspose.tasks.visualization/barstyle/topbartextconverter/) { get; set; } | Ottiene o imposta il convertitore definito dall'utente per ottenere il testo da visualizzare nella parte superiore della barra dell'attività. Sovrascrive il valore della proprietà [`TopField`](./topfield/). |
| [TopField](../../aspose.tasks.visualization/barstyle/topfield/) { get; set; } | Ottiene o imposta un campo da visualizzare in alto della barra. |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


