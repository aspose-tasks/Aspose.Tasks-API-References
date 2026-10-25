---
title: "MPPSaveOptions.WriteFilters"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MPPSaveOptions. Возвращает или задает значение, указывающее, следует ли записывать данные фильтров при сохранении проекта в формат MPP. Данные фильтров включают коллекции Project.TaskFilters и Project.ResourceFilters."
type: docs
weight: 50
url: /ru/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Получает или задает значение, указывающее, следует ли записывать данные фильтров при сохранении проекта в формат MPP. Данные фильтров включают коллекции Project.TaskFilters и Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Примечания

В настоящее время поддерживается для форматов MSP 2010 и новее.

## Примеры

Показывает, как добавить и сохранить новый фильтр задач в проект MPP.

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

### См. также

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


