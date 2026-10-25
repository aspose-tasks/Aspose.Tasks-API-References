---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "MPPSaveOptions özelliği. Bir projeyi MPP formatında kaydederken filtre verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Filtre verileri Project.TaskFilters ve Project.ResourceFilters koleksiyonlarını içerir."
type: docs
weight: 50
url: /tr/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Projeyi MPP formatında kaydederken filtre verilerinin yazılıp yazılmayacağını gösteren bir değeri alır veya ayarlar. Filtre verileri Project.TaskFilters ve Project.ResourceFilters koleksiyonlarını içerir.

```csharp
public bool WriteFilters { get; set; }
```

## Açıklamalar

Şu anda MSP 2010 ve daha yeni formatlar için desteklenmektedir.

## Örnekler

Yeni görev filtresinin MPP projesine nasıl ekleneceğini ve kaydedileceğini gösterir.

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

### Ayrıca Bakınız

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


