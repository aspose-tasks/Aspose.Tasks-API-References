---
title: "MPPSaveOptions.WriteFilters"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah data filter harus ditulis saat menyimpan proyek ke format MPP. Data filter mencakup koleksi Project.TaskFilters dan Project.ResourceFilters."
type: docs
weight: 50
url: /id/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan menulis data filter saat menyimpan proyek ke format MPP. Data filter mencakup koleksi Project.TaskFilters dan Project.ResourceFilters.

```csharp
public bool WriteFilters { get; set; }
```

## Catatan

Saat ini didukung untuk format MSP 2010 atau yang lebih baru.

## Contoh

Menampilkan cara menambahkan dan menyimpan filter tugas baru ke proyek MPP.

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

### Lihat Juga

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


