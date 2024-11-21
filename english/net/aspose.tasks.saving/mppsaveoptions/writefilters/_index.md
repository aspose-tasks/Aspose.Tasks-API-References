---
title: MPPSaveOptions.WriteFilters
second_title: Aspose.Tasks for .NET API Reference
description: MPPSaveOptions property. Gets or sets a value indicating whether to write filter data when saving a project to MPP for format. Filter data includes Project.TaskFilters and Project.ResourceFilters collections
type: docs
weight: 50
url: /net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Gets or sets a value indicating whether to write filter data when saving a project to MPP for format. Filter data includes Project.TaskFilters and Project.ResourceFilters collections.

```csharp
public bool WriteFilters { get; set; }
```

## Remarks

Currently supported for MSP 2010 or newer formats.

## Examples

Shows how to add and save new task filter to MPP project.

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

### See Also

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


