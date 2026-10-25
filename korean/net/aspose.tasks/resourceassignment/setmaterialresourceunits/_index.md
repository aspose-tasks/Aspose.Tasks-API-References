---
title: "ResourceAssignment.SetMaterialResourceUnits"
second_title: "Aspose.Tasks for .NET API 참조"
description: "ResourceAssignment 메서드. 가변 재료 소비가 있는 물리적 자원의 할당을 위해 단위를 설정합니다. 가변 재료 소비란 할당 기간이 변경됨에 따라 사용되는 재료 양이 비례적으로 변함을 의미합니다."
type: docs
weight: 760
url: /ko/net/aspose.tasks/resourceassignment/setmaterialresourceunits/
---
## ResourceAssignment.SetMaterialResourceUnits method

가변 재료 소비가 있는 물리적 리소스 할당에 대한 단위를 설정합니다. 가변 재료 소비란 할당 기간이 변경됨에 따라 사용되는 재료 수량이 비례하여 변함을 의미합니다.

```csharp
public void SetMaterialResourceUnits(double units, RateScaleType rateScaleType)
```

| 매개변수 | 형식 | 설명 |
| --- | --- | --- |
| 단위 | Double | 해당 기간에 누적된 단위 수. |
| rateScaleType | RateScaleType | 단위 값이 누적되는 기간. |

### 예외

| 예외 | 조건 |
| --- | --- |
| InvalidOperationException | 메서드가 비물리적 자원 할당에 대해 호출되는 경우. |

## 비고

예를 들어, '123/월'을 설정하려면 SetUnitsScaled(123D, RateScaleType.Month)를 호출해야 합니다.

## 예제

재료 리소스 할당에 대해 가변 재료 소비량(예: '10/day' 또는 '1/week')을 설정하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// '1/week' 재료 소비량을 설정하고 싶다고 가정합니다.
materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);
```

### 또 보기

* enum [RateScaleType](../../ratescaletype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


