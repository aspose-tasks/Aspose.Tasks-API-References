---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "MPPSaveOptions プロパティ。 プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を取得または設定します。 フィルタ データには Project.TaskFilters および Project.ResourceFilters コレクションが含まれます"
type: docs
weight: 50
url: /ja/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

プロジェクトを MPP 形式で保存する際にフィルタ データを書き込むかどうかを示す値を取得または設定します。 フィルタ データには Project.TaskFilters および Project.ResourceFilters コレクションが含まれます。

```csharp
public bool WriteFilters { get; set; }
```

## 備考

現在、MSP 2010 以降の形式がサポートされています。

## 例

新しいタスク フィルターを MPP プロジェクトに追加して保存する方法を示します。

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

### 関連項目

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


