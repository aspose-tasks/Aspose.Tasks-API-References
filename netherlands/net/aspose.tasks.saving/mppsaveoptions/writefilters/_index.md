---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP‑formaat. Filtergegevens omvatten de collecties Project.TaskFilters en Project.ResourceFilters."
type: docs
weight: 50
url: /nl/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Haalt op of stelt een waarde in die aangeeft of filtergegevens moeten worden weggeschreven bij het opslaan van een project naar MPP-formaat. Filtergegevens omvatten de collecties Project.TaskFilters en Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Opmerkingen

Momenteel ondersteund voor MSP 2010 of nieuwere formaten.

## Voorbeelden

Toont hoe een nieuw taakfilter toe te voegen en op te slaan in een MPP‑project.

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

### Zie ook

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


