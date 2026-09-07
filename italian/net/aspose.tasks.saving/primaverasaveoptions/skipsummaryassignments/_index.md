---
title: "PrimaveraSaveOptions.SkipSummaryAssignments"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà PrimaveraSaveOptions. Ottiene o imposta un valore che indica se le assegnazioni di risorse ai compiti riepilogo devono essere ignorate durante l'esportazione"
type: docs
weight: 60
url: /it/net/aspose.tasks.saving/primaverasaveoptions/skipsummaryassignments/
---
## PrimaveraSaveOptions.SkipSummaryAssignments property

Ottiene o imposta un valore che indica se le assegnazioni di risorse alle attività riepilogo devono essere omesse durante l'esportazione.

```csharp
public bool SkipSummaryAssignments { get; set; }
```

## Osservazioni

Il software Primavera non supporta le assegnazioni di risorse alle attività di riepilogo (WBS). Pertanto, l'esportazione di tali assegnazioni può generare un file non valido secondo il modello di Primavera. Se vero, le assegnazioni alle attività di riepilogo vengono omesse durante l'esportazione. Se falso (il valore predefinito), viene sollevata un'eccezione se durante l'esportazione viene incontrata un'assegnazione a un'attività di riepilogo.

## Esempi

Mostra come usare il flag SkipSummaryAssignments.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var resource = project.Resources.Add("Resource");

var summaryTask = project.RootTask.Children.Add("Summary");
summaryTask.Children.Add("Task");

// Primavera non supporta le assegnazioni di risorse alle attività di riepilogo.
// Quindi l'esportazione di tali assegnazioni nel formato Primavera può generare file che non possono essere importati in Primavera.
var assignment = project.ResourceAssignments.Add(summaryTask, resource);

var options = new PrimaveraXmlSaveOptions();
options.SkipSummaryAssignments = true;
project.Save(OutDir + "UseSkipSummaryAssignments_out.xml", options);
```

### Vedi anche

* class [PrimaveraSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../primaverasaveoptions/)
* assembly [Aspose.Tasks](../../../)


