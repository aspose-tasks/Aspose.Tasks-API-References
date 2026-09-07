---
title: "Enum Shape"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.Shape enum. Forma di un marcatore all'inizio o alla fine dello stile della barra da renderizzare quando si salva la visualizzazione dei dati in alcuni di SaveFileFormat"
type: docs
weight: 3360
url: /it/net/aspose.tasks.visualization/shape/
---
## Shape enumeration

Forma di un marcatore all'inizio o alla fine dello stile della barra da renderizzare quando si salva la visualizzazione dei dati in alcuni di [`SaveFileFormat`](../../aspose.tasks.saving/savefileformat/).

```csharp
public enum Shape
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| None | `0` | Indica la forma Nessuna. |
| VerticalLine | `1` | Indica la forma Linea verticale. |
| Pentagon | `2` | Indica la forma Pentagono. |
| Triangle | `3` | Indica la forma Triangolo. |
| LeftBracket | `4` | Indica la forma Parentese sinistro. |
| RightBracket | `5` | Indica la forma Parentese destro. |
| ArrowDown | `6` | Indica la forma ArrowDown. |
| LeftFade | `7` | Indica la forma Sfumatura sinistra. |
| RightFade | `8` | Indica la forma Sfumatura destra. |
| Diamond | `9` | Indica la forma Diamante. |
| Circle | `10` | Indica la forma Cerchio. |

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


