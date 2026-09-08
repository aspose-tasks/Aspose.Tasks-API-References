---
title: "MPPSaveOptions.WriteViewData"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MPPSaveOptions 속성. 프로젝트를 MPP 형식으로 저장할 때 보기 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 보기 데이터에는 Project.Views 필터와 Tables 컬렉션이 포함됩니다."
type: docs
weight: 80
url: /ko/net/aspose.tasks.saving/mppsaveoptions/writeviewdata/
---
## MPPSaveOptions.WriteViewData property

MPP 형식으로 프로젝트를 저장할 때 보기 데이터를 기록할지 여부를 나타내는 값을 가져오거나 설정합니다. 보기 데이터에는 Project.Views, Filters 및 Tables 컬렉션이 포함됩니다.

```csharp
public bool WriteViewData { get; set; }
```

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


