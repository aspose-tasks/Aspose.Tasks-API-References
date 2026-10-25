---
title: "UsageView.DisplayShortDetailHeaderNames"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "UsageView proprietà. Ottiene o imposta un valore che indica se visualizzare o meno i nomi brevi delle intestazioni di dettaglio"
type: docs
weight: 40
url: /it/net/aspose.tasks/usageview/displayshortdetailheadernames/
---
## UsageView.DisplayShortDetailHeaderNames property

Ottiene o imposta un valore che indica se visualizzare o meno i nomi brevi dell'intestazione dei dettagli.

```csharp
public bool DisplayShortDetailHeaderNames { get; set; }
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


