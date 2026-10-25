---
title: "MPPSaveOptions.WriteFilters"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MPPSaveOptions 속성. 프로젝트를 MPP 형식으로 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 필터 데이터에는 Project.TaskFilters 및 Project.ResourceFilters 컬렉션이 포함됩니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks.saving/mppsaveoptions/writefilters/
---
## MPPSaveOptions.WriteFilters property

MPP 형식으로 프로젝트를 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 필터 데이터에는 Project.TaskFilters 및 Project.ResourceFilters 컬렉션이 포함됩니다.

```csharp
public bool WriteFilters { get; set; }
```

## 비고

현재 MSP 2010 이상 형식에서 지원됩니다.

## 예제

새 작업 필터를 MPP 프로젝트에 추가하고 저장하는 방법을 보여줍니다.

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

### 또 보기

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


