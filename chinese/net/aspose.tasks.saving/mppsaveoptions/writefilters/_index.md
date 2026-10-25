---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。过滤器数据包括 Project.TaskFilters 和 Project.ResourceFilters 集合。"
type: docs
weight: 50
url: /zh/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

获取或设置一个值，指示在将项目保存为 MPP 格式时是否写入过滤器数据。过滤器数据包括 Project.TaskFilters 和 Project.ResourceFilters 集合。

```csharp
public bool WriteFilters { get; set; }
```

## 备注

当前支持 MSP 2010 或更高版本的格式。

## 示例

展示如何向 MPP 项目添加并保存新的任务过滤器。

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

### 另见

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


