---
title: "Asn.RateScale"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Asn 필드. 물자 리소스 할당의 사용률에 대한 시간 단위. 정의되지 않은 경우 0을 반환합니다"
type: docs
weight: 410
url: /ko/net/aspose.tasks/asn/ratescale/
---
## Asn.RateScale field

자재 리소스 할당의 사용률에 대한 시간 단위. 정의되지 않은 경우 0을 반환합니다.

```csharp
public static readonly Key<RateScaleType, AsnKey> RateScale;
```

## 예제

재료 리소스 할당에 대해 가변 재료 소비량(예: '10/day' 또는 '1/week')을 설정하려는 경우 할당의 비율 스케일을 사용하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "New project 2013.mpp");

var task = project.RootTask.Children.Add("t1");

var materialResource = project.Resources.Add("materialResource");
materialResource.Set(Rsc.Type, ResourceType.Material);

var nonMaterialResource = project.Resources.Add("nonMaterialResource");
nonMaterialResource.Set(Rsc.Type, ResourceType.Work);

var materialResourceAssignment = project.ResourceAssignments.Add(task, materialResource);

// '1/week' 재료 소비량을 설정하고 싶다고 가정합니다.
// 시간당 비율을 Units 속성에 설정해야 하므로 1D를 주당 시간 수로 나눕니다.
materialResourceAssignment.Set(Asn.Units, 1D / 40);
materialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

// 24.4부터는 이 작업을 한 메서드를 호출하여 수행할 수 있다는 점에 유의하세요:
// materialResourceAssignment.SetMaterialResourceUnits(1D, RateScaleType.Week);

var nonMaterialResourceAssignment = project.ResourceAssignments.Add(task, nonMaterialResource);
nonMaterialResourceAssignment.Set(Asn.RateScale, RateScaleType.Week);

project.Save(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp", SaveFileFormat.Mpp);

var resavedProject = new Project(OutDir + "ReadWriteRateScaleForResourceAssignment_out.mpp");

var resavedMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(2);
Console.WriteLine(resavedMaterialResourceAssignment.Get(Asn.RateScale));

// 비제로 비율 스케일 값을 가질 수 있는 것은 재료 리소스 할당뿐입니다.
var resavedNonMaterialResourceAssignment = resavedProject.ResourceAssignments.GetByUid(3);
Console.WriteLine(resavedNonMaterialResourceAssignment.Get(Asn.RateScale));
```

### 또 보기

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateScaleType](../../ratescaletype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


