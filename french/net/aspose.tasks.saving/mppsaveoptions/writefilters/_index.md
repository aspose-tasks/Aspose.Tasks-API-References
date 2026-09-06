---
title: "MPPSaveOptions.WriteFilters"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. Les données de filtre incluent les collections Project.TaskFilters et Project.ResourceFilters."
type: docs
weight: 50
url: /fr/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Obtient ou définit une valeur indiquant s'il faut écrire les données de filtre lors de l'enregistrement d'un projet au format MPP. Les données de filtre comprennent les collections Project.TaskFilters et Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Remarques

Actuellement pris en charge pour les formats MSP 2010 ou plus récents.

## Exemples

Montre comment ajouter et enregistrer un nouveau filtre de tâche dans un projet MPP.

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

### Voir aussi

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


