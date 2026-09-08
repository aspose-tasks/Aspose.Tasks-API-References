---
title: "클래스 MPPSaveOptions"
second_title: "Aspose.Tasks for .NET API 참조"
description: "Aspose.Tasks.Saving.MPPSaveOptions 클래스. 프로젝트 데이터를 MPP로 저장할 때 추가 옵션을 지정할 수 있습니다."
type: docs
weight: 2050
url: /ko/net/aspose.tasks.saving/mppsaveoptions/
---
## MPPSaveOptions class

프로젝트 데이터를 MPP로 저장할 때 추가 옵션을 지정할 수 있습니다.

```csharp
public class MPPSaveOptions : SimpleSaveOptions
```

## 생성자

| 이름 | 설명 |
| --- | --- |
| [MPPSaveOptions](mppsaveoptions/)() | `MPPSaveOptions` 클래스의 새 인스턴스를 초기화합니다. |

## 속성

| 이름 | 설명 |
| --- | --- |
| [ClearVba](../../aspose.tasks.saving/mppsaveoptions/clearvba/) { get; set; } | 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 가져오거나 설정합니다. |
| [ProtectionPassword](../../aspose.tasks.saving/mppsaveoptions/protectionpassword/) { get; set; } | 결과 MPP 파일을 보호하는 데 사용되는 비밀번호를 가져오거나 설정합니다. 현재 MS Project 2010 및 이후 형식에서 지원됩니다. null 값은 프로젝트 파일이 보호되지 않음을 나타냅니다. |
| [RemoveInvalidAssignments](../../aspose.tasks.saving/mppsaveoptions/removeinvalidassignments/) { get; set; } | MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 가져오거나 설정합니다. MS Project는 각 작업에 대해 빈 리소스 할당을 생성합니다. 저장 시 이를 제거하려면 이 플래그를 true로 설정하십시오. |
| [SaveFormat](../../aspose.tasks.saving/simplesaveoptions/saveformat/) { get; } | 이 저장 옵션 개체가 사용될 경우 문서가 저장되는 형식을 가져오거나 설정합니다. |
| [TasksComparer](../../aspose.tasks.saving/simplesaveoptions/taskscomparer/) { get; set; } | 간트 차트 및 작업 시트 차트에서 작업을 정렬하기 위한 비교자를 가져오거나 설정합니다. |
| [TasksFilter](../../aspose.tasks.saving/simplesaveoptions/tasksfilter/) { get; set; } | 간트, 작업 시트 및 작업 사용 차트에 렌더링된 작업을 필터링하는 데 사용되는 조건을 가져오거나 설정합니다. |
| [WriteFilters](../../aspose.tasks.saving/mppsaveoptions/writefilters/) { get; set; } | MPP 형식으로 프로젝트를 저장할 때 필터 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 필터 데이터에는 Project.TaskFilters 및 Project.ResourceFilters 컬렉션이 포함됩니다. |
| [WriteGroups](../../aspose.tasks.saving/mppsaveoptions/writegroups/) { get; set; } | MPP 형식으로 프로젝트를 저장할 때 그룹 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 그룹 데이터에는 Project.TaskGroups 및 Project.ResourceGroups 컬렉션이 포함됩니다. |
| [WriteVba](../../aspose.tasks.saving/mppsaveoptions/writevba/) { get; set; } | MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 가져오거나 설정합니다. 현재 VbaModule.SourceCode의 기록이 지원됩니다. |
| [WriteViewData](../../aspose.tasks.saving/mppsaveoptions/writeviewdata/) { get; set; } | MPP 형식으로 프로젝트를 저장할 때 보기 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 보기 데이터에는 Project.Views, Filters 및 Tables 컬렉션이 포함됩니다. |

## 예제

프로젝트를 스트림에 MPP 파일로 저장하는 방법을 보여줍니다.

```csharp
using (var stream = new FileStream(OutDir + "EmptyProjectSaveStream_out.xml", FileMode.Create, FileAccess.Write))
{
    var project = new Project(DataDir + "EstimatedMilestoneTasks.mpp");

    // 저장 옵션을 생성합니다.
    SimpleSaveOptions options = new MPPSaveOptions
    {
        // MPP로 저장할 때 잘못된 리소스 할당을 제거할지 여부를 나타내는 값을 설정합니다.
        RemoveInvalidAssignments = true
    };

    // 옵션을 사용하여 MPP를 저장합니다.
    project.Save(stream, options);
}
```

### 또 보기

* class [SimpleSaveOptions](../simplesaveoptions/)
* namespace [Aspose.Tasks.Saving](../../aspose.tasks.saving/)
* assembly [Aspose.Tasks](../../)


