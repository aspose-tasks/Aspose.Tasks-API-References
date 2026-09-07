---
title: "UsageView.AlignDetailsData"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "UsageView proprietà. Ottiene o imposta l'allineamento dei dati di dettaglio"
type: docs
weight: 10
url: /it/net/aspose.tasks/usageview/aligndetailsdata/
---
## UsageView.AlignDetailsData property

Ottiene o imposta l'allineamento dei dati dei dettagli.

```csharp
public HorizontalStringAlignment AlignDetailsData { get; set; }
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

* enum [HorizontalStringAlignment](../../../aspose.tasks.visualization/horizontalstringalignment/)
* class [UsageView](../)
* namespace [Aspose.Tasks](../../usageview/)
* assembly [Aspose.Tasks](../../../)


