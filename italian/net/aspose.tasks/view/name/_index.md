---
title: "View.Name"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà View. Ottiene o imposta il nome di un oggetto View"
type: docs
weight: 50
url: /it/net/aspose.tasks/view/name/
---
## View.Name property

Ottiene o imposta il nome di un oggetto View.

```csharp
public string Name { get; set; }
```

## Esempi

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


