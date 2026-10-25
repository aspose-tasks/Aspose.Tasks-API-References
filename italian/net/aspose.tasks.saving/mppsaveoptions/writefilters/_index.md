---
title: "MPPSaveOptions.WriteFilters"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP. I dati dei filtri includono le collezioni Project.TaskFilters e Project.ResourceFilters."
type: docs
weight: 50
url: /it/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Ottiene o imposta un valore che indica se scrivere i dati dei filtri durante il salvataggio di un progetto in formato MPP. I dati dei filtri includono le collezioni Project.TaskFilters e Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Osservazioni

Attualmente supportato per i formati MSP 2010 o successivi.

## Esempi

Mostra come aggiungere e salvare un nuovo filtro attività in un progetto MPP.

```csharp
Project project = new Project();

project.TaskFilters.Clear();
project.ResourceFilters.Clear();

var filter = new Filter();
filter.Name = "New Task Filter";
filter.FilterType = ItemType.TaskItem;
filter.ShowInMenu = true;
filter.ShowRelatedSummaryRows = true;

filter.Criteria = new FilterCriteria();

var criteria1 = new FilterCriteria();
criteria1.Field = Field.TaskNumber13;
criteria1.Test = FilterComparisonType.IsLessThan;
criteria1.Values[0] = 34.3D;

filter.Criteria.CriteriaRows.Add(criteria1);
project.TaskFilters.Add(filter);

SimpleSaveOptions options = new MPPSaveOptions() { WriteFilters = true };
project.Save(OutDir + "output_new_filter.mpp", options);
```

### Vedi anche

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


