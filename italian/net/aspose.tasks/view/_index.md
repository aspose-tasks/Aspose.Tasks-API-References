---
title: "Classe View"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.View. Rappresenta una vista in Project"
type: docs
weight: 2890
url: /it/net/aspose.tasks/view/
---
## View class

Rappresenta una vista in Project.

```csharp
public class View : IComparable<View>
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [View](view/#constructor)() | Inizializza una nuova istanza della classe `View`. |
| [View](view/#constructor_1)(ViewScreen) | Inizializza una nuova istanza della classe `View`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| [Filter](../../aspose.tasks/view/filter/) { get; set; } | Ottiene o imposta un filtro utilizzato in una singola vista. |
| [Group](../../aspose.tasks/view/group/) { get; set; } | Ottiene o imposta un gruppo della singola vista. |
| [HighlightFilter](../../aspose.tasks/view/highlightfilter/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project evidenzia il filtro per una singola vista. |
| [Name](../../aspose.tasks/view/name/) { get; set; } | Ottiene o imposta il nome di un oggetto View. |
| [PageInfo](../../aspose.tasks/view/pageinfo/) { get; } | Ottiene un'istanza della classe [`PageInfo`](./pageinfo/). Rappresenta i dati di impostazione della pagina presenti nel formato file mpp. |
| [ParentProject](../../aspose.tasks/view/parentproject/) { get; } | Ottiene il genitore dell'oggetto View. Solo lettura [`Project`](../project/). |
| [Screen](../../aspose.tasks/view/screen/) { get; } | Ottiene il tipo di schermo per la singola vista. Solo lettura [`ViewScreen`](../viewscreen/). |
| [ShowInMenu](../../aspose.tasks/view/showinmenu/) { get; set; } | Ottiene o imposta un valore che indica se Microsoft Project mostra il nome della singola vista nelle liste a discesa Vista o Altre viste nel Ribbon. |
| [Table](../../aspose.tasks/view/table/) { get; set; } | Ottiene o imposta una tabella della singola vista. |
| [Type](../../aspose.tasks/view/type/) { get; } | Ottiene il tipo di elemento nella singola vista, come attività o risorse. Solo lettura [`ItemType`](../itemtype/). |
| [Uid](../../aspose.tasks/view/uid/) { get; } | Ottiene l'identificatore univoco di una vista. |
| [VisualObjectsPlacements](../../aspose.tasks/view/visualobjectsplacements/) { get; } | Ottiene una raccolta di oggetti che rappresentano la posizione e l'aspetto di [`OleObject`](../oleobject/) nella vista. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [CompareTo](../../aspose.tasks/view/compareto/)(View) | Confronta l'istanza corrente con un altro oggetto dello stesso tipo e restituisce un intero che indica se l'istanza corrente precede, segue o si trova nella stessa posizione nell'ordine di ordinamento rispetto all'altro oggetto. |
| override [Equals](../../aspose.tasks/view/equals/)(object) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| override [GetHashCode](../../aspose.tasks/view/gethashcode/)() | Restituisce un valore di codice hash per l'istanza della classe [`Resource`](../resource/). |
| [operator ==](../../aspose.tasks/view/op_equality/) | Restituisce un valore che indica se questa istanza è uguale a un oggetto specificato. |
| [operator &gt;](../../aspose.tasks/view/op_greaterthan/) | Restituisce un valore che indica se questa istanza è maggiore di un oggetto specificato. |
| [operator &gt;=](../../aspose.tasks/view/op_greaterthanorequal/) | Restituisce un valore che indica se questa istanza è maggiore o uguale a un oggetto specificato. |
| [operator !=](../../aspose.tasks/view/op_inequality/) | Restituisce un valore che indica se questa istanza non è uguale a un oggetto specificato. |
| [operator &lt;](../../aspose.tasks/view/op_lessthan/) | Restituisce un valore che indica se questa istanza è minore di un oggetto specificato. |
| [operator &lt;=](../../aspose.tasks/view/op_lessthanorequal/) | Restituisce un valore che indica se questa istanza è minore o uguale a un oggetto specificato. |

## Esempi

Mostra come lavorare con la vista di Project e aggiungere una colonna alla vista predefinita (che viene mostrata quando un file MPP è aperto in MS Project).

```csharp
// crea un progetto vuoto senza viste
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// Modifica la vista predefinita (è una vista diagramma di Gantt).
// Oppure puoi selezionare la vista per nome o tramite la schermata Vista usando la collezione project.View.
var view = (GanttChartView) project.DefaultView;

TableField newColumn = new TableField()
{
    AlignData = HorizontalStringAlignment.Center,
    Title = "My new column",
    Width = 30,
    Field = Field.TaskActualDuration
};

view.Table.TableFields.Add(newColumn);

// Il flag WriteViewData dovrebbe essere usato per persistere le modifiche alle proprietà della vista.
project.Save(OutDir + "ModifyView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
```

Mostra come lavorare con le viste di MS Project.

```csharp
// crea un progetto vuoto senza viste
var project = new Project();
project.Set(Prj.Name, "Test View Project");

// crea una vista standard di diagramma di Gantt
View view = new GanttChartView();

// imposta alcune proprietà della vista
// imposta un valore che indica se Microsoft Project mostra il nome della singola vista nella View o nelle liste a discesa Other Views nel Ribbon
view.ShowInMenu = true;
// imposta un valore che indica se Microsoft Project evidenzia il filtro per una singola vista
view.HighlightFilter = true;

// la scrittura delle proprietà successive non è supportata
// imposta il filtro utilizzato in una singola vista
view.Filter = null;
// imposta il gruppo della singola vista
view.Group = null;
// imposta la tabella della singola vista
view.Table = null;

// regoliamo alcune impostazioni della vista
// imposta il numero delle prime colonne da stampare su tutte le pagine
view.PageInfo.PageViewSettings.FirstColumnsCount = 4;
// imposta un valore che indica se stampare un numero specificato di prime colonne su tutte le pagine
view.PageInfo.PageViewSettings.PrintFirstColumnsCountOnAllPages = true;

// aggiungi la vista al nostro progetto
project.Views.Add(view);

// Il flag WriteViewData dovrebbe essere usato per persistere le modifiche di project.Views.
project.Save(OutDir + "WorkWithView_output.mpp", new Saving.MPPSaveOptions
{
    WriteViewData = true
});
// verifichiamo alcune proprietà della vista appena aggiunta
// stampa l'identificatore univoco di una vista
Console.WriteLine("View Uid: " + view.Uid);
// stampa il tipo di schermo per la singola vista
Console.WriteLine("View Screen: " + view.Screen);
Console.WriteLine("View Type: " + view.Type);
Console.WriteLine("Parent Project of the view: " + view.ParentProject.Get(Prj.Name));
```

### Vedi anche

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


