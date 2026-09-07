---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "MPPSaveOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP‑Format geschrieben werden sollen. Filterdaten umfassen die Sammlungen Project.TaskFilters und Project.ResourceFilters."
type: docs
weight: 50
url: /de/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Gibt einen Wert zurück oder legt ihn fest, der angibt, ob Filterdaten beim Speichern eines Projekts im MPP‑Format geschrieben werden sollen. Filterdaten umfassen die Sammlungen Project.TaskFilters und Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Hinweise

Derzeit unterstützt für MSP‑2010‑ oder neuere Formate.

## Beispiele

Zeigt, wie ein neuer Aufgabenfilter zu einem MPP‑Projekt hinzugefügt und gespeichert wird.

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

### Siehe auch

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


