---
title: "XlsxOptions.ResourceView"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà XlsxOptions. Ottiene o imposta un elenco delle colonne della vista delle risorse da rendere ResourceViewColumn"
type: docs
weight: 40
url: /it/net/aspose.tasks.saving/xlsxoptions/resourceview/
---
## XlsxOptions.ResourceView property

Ottiene o imposta un elenco delle colonne della vista risorsa da renderizzare ([`ResourceViewColumn`](../../../aspose.tasks.visualization/resourceviewcolumn/)).

```csharp
public ProjectView ResourceView { get; set; }
```

## Esempi

Mostra come salvare un progetto in un file XLSX utilizzando le opzioni &lt;see cref="P:Aspose.Tasks.Saving.XlsxOptions"&gt;Days&lt;/see&gt;.

```csharp
var project = new Project(DataDir + "CreateProject2.mpp");

var options = new XlsxOptions();

// Aggiungi le colonne desiderate del diagramma di Gantt
var col = new GanttChartColumn("WBS", 100, delegate(Task task) { return task.Get(Tsk.WBS); });
options.View.Columns.Add(col);

// Aggiungi le colonne desiderate della vista risorse
var rscCol = new ResourceViewColumn("Cost center", 100, delegate(Resource resource) { return resource.Get(Rsc.CostCenter); });
options.ResourceView.Columns.Add(rscCol);

// Aggiungi le colonne desiderate della vista assegnazioni
var assnCol = new AssignmentViewColumn("Notes", 200, delegate(ResourceAssignment assignment) { return assignment.Get(Asn.NotesText); });
options.AssignmentView.Columns.Add(assnCol);

// imposta codifica
options.Encoding = Encoding.Unicode;

project.Save(OutDir + "UsingXlsxOptions_out.xlsx", options);
```

### Vedi anche

* class [ProjectView](../../../aspose.tasks.visualization/projectview/)
* class [XlsxOptions](../)
* namespace [Aspose.Tasks.Saving](../../xlsxoptions/)
* assembly [Aspose.Tasks](../../../)


