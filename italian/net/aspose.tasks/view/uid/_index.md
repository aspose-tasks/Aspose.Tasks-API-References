---
title: "View.Uid"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà View. Ottiene l'identificatore univoco di una vista"
type: docs
weight: 120
url: /it/net/aspose.tasks/view/uid/
---
## View.Uid property

Ottiene l'identificatore univoco di una vista.

```csharp
public int Uid { get; }
```

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

* class [View](../)
* namespace [Aspose.Tasks](../../view/)
* assembly [Aspose.Tasks](../../../)


