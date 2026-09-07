---
title: "Project.DefaultView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà del progetto. Ottiene o imposta la vista predefinita del progetto"
type: docs
weight: 360
url: /it/net/aspose.tasks/project/defaultview/
---
## Project.DefaultView property

Ottiene o imposta la vista predefinita del progetto.

```csharp
public View DefaultView { get; set; }
```

## Esempi

Mostra come lavorare con la vista predefinita di un progetto.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// Ottieni vista predefinita
UsageView view = (TaskUsageView)project.DefaultView;

// La colonna dell'intestazione dei dettagli non verrà visualizzata
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// Visualizza colonna dell'intestazione dei dettagli
view.DisplayDetailsHeaderColumn = true;

// Ripeti l'intestazione dei dettagli su tutte le righe delle assegnazioni
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

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

### Vedi anche

* class [View](../../view/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


