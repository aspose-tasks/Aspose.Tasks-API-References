---
title: "UsageView.DisplayDetailsHeaderColumn"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "proprietà UsageView. Ottiene o imposta un valore che indica se visualizzare o meno la colonna dell'intestazione dei dettagli nella visualizzazione."
type: docs
weight: 30
url: /it/net/aspose.tasks/usageview/displaydetailsheadercolumn/
---
## UsageView.DisplayDetailsHeaderColumn property

Ottiene o imposta un valore che indica se visualizzare o meno la colonna intestazione dei dettagli nella vista.

```csharp
public bool DisplayDetailsHeaderColumn { get; set; }
```

## Esempi

Mostra come rendere la vista utilizzo attività con dettagli.

```csharp
var project = new Project(DataDir + "TaskUsageViewWithDetails.mpp");

// ottieni la vista
UsageView view = (TaskUsageView)project.DefaultView;

// la colonna dell'intestazione dei dettagli non verrà visualizzata
view.DisplayDetailsHeaderColumn = false;
view.RepeatDetailsHeaderOnAllRows = false;
view.DisplayShortDetailHeaderNames = false;
view.AlignDetailsData = HorizontalStringAlignment.Near;
project.Save(OutDir + "task usage1_out.pdf", SaveFileFormat.Pdf);

// visualizza la colonna dell'intestazione dei dettagli
view.DisplayDetailsHeaderColumn = true;

// ripeti l'intestazione dei dettagli su tutte le righe delle assegnazioni
view.RepeatDetailsHeaderOnAllRows = true;
view.AlignDetailsData = HorizontalStringAlignment.Far;
project.Save(OutDir + "task usage2_out.pdf", SaveFileFormat.Pdf);
```

### Vedi anche

* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


