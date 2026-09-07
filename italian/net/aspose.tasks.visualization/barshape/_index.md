---
title: "Enum BarShape"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Aspose.Tasks.Visualization.BarShape enum. Forma di un rettangolo della barra."
type: docs
weight: 2950
url: /it/net/aspose.tasks.visualization/barshape/
---
## BarShape enumeration

Forma del rettangolo della barra.

```csharp
public enum BarShape
```

### Valori

| Nome | Valore | Descrizione |
| --- | --- | --- |
| Full | `0` | Indica la forma a rettangolo pieno. |
| HalfHeight | `1` | Indica la forma a rettangolo di metà altezza allineata in alto. |
| HalfHeightBottom | `2` | Indica la forma a rettangolo di metà altezza allineata in basso. |
| Thin | `3` | Indica la forma a linea allineata al centro. |
| None | `4` | Indica la forma di barra Nessuna. |
| Middle | `5` | Indica la forma a linea allineata al centro. |
| LineBottom | `6` | Indica la forma a linea allineata in basso. |
| LineTop | `7` | Indica la forma a linea allineata in alto. |

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


