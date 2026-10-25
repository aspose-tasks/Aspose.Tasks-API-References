---
title: "MPPSaveOptions.ClearVba"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MPPSaveOptions 속성. 프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 가져오거나 설정합니다."
type: docs
weight: 20
url: /ko/net/aspose.tasks.saving/mppsaveoptions/clearvba/
---
## MPPSaveOptions.ClearVba property

프로젝트를 MPP 형식으로 저장할 때 기존 VBA 매크로 데이터를 제거할지 여부를 나타내는 값을 가져오거나 설정합니다.

```csharp
public bool ClearVba { get; set; }
```

## 예제

MPP 파일에서 VBA 매크로를 제거하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

### 또 보기

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


