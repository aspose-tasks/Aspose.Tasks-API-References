---
title: "Classe ResourceViewColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Classe Aspose.Tasks.Visualization.ResourceViewColumn. Classe di visualizzazione dei progetti utilizzata nella visualizzazione ResourceUsage e nella visualizzazione ResourceSheet"
type: docs
weight: 3350
url: /it/net/aspose.tasks.visualization/resourceviewcolumn/
---
## ResourceViewColumn class

Classe di visualizzazione del progetto usata nella visualizzazione ResourceUsage e nella visualizzazione ResourceSheet.

```csharp
public sealed class ResourceViewColumn : ViewColumn
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ResourceViewColumn](resourceviewcolumn/#constructor)(int, Field) | Inizializza una nuova istanza della classe `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_1)(string, int, ResourceToColumnTextConverter) | Inizializza una nuova istanza della classe `ResourceViewColumn`. |
| [ResourceViewColumn](resourceviewcolumn/#constructor_2)(string, int, ResourceToColumnTextConverter, Field) | Inizializza una nuova istanza della classe `ResourceViewColumn`. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [Field](../../aspose.tasks.visualization/resourceviewcolumn/field/) { get; set; } | Campo colonna. [`Field`](./field/). |
| [Name](../../aspose.tasks.visualization/viewcolumn/name/) { get; } | Ottiene il nome della colonna. |
| [StringAlignment](../../aspose.tasks.visualization/viewcolumn/stringalignment/) { get; set; } | Ottiene o imposta l'allineamento del testo (può essere uno dei valori dell'enumerazione [`HorizontalStringAlignment`](../horizontalstringalignment/)). |
| [TextStyleModificationCallback](../../aspose.tasks.visualization/viewcolumn/textstylemodificationcallback/) { get; set; } | Ottiene o imposta il callback che può essere usato per personalizzare l'aspetto delle celle della colonna. |
| [Width](../../aspose.tasks.visualization/viewcolumn/width/) { get; } | Ottiene la larghezza della colonna. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [GetColumnText](../../aspose.tasks.visualization/resourceviewcolumn/getcolumntext/)(Resource) | Converte la risorsa corrente nel testo della colonna. |

## Esempi

Mostra come aggiungere colonne di visualizzazione delle risorse da esportare.

```csharp
var project = new Project(DataDir + "Project2.mpp");
var resource = project.Resources.GetById(1);

var options = new PdfSaveOptions();
var columns = new List<ViewColumn>
{
    new ResourceViewColumn(100, Field.ResourceName),
    new ResourceViewColumn(100, Field.ResourceActualWork),
    new ResourceViewColumn(100, Field.ResourceCost),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }),
    new ResourceViewColumn(
        "Resource Cost2", 
        80,
        delegate(Resource res)
        {
            return res.Get(Rsc.Cost).ToString(CultureInfo.InvariantCulture);
        }, 
        Field.ResourceCost2)
};

// itera sulle colonne
foreach (var column in columns)
{
    var col = (ResourceViewColumn)column;
    Console.WriteLine("Column Name: " + col.Name);
    Console.WriteLine("Column Field: " + col.Field);
    Console.WriteLine("Column Text: " + col.GetColumnText(resource));
    Console.WriteLine();
}

options.View = new ProjectView(columns);
options.PresentationFormat = PresentationFormat.ResourceUsage;
project.Save(OutDir + "WorkWithAssignmentViewColumn_out.pdf", options);
```

### Vedi anche

* class [ViewColumn](../viewcolumn/)
* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


