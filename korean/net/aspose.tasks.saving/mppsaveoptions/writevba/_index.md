---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET API 참조"
description: "MPPSaveOptions 속성. MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 가져오거나 설정합니다. 현재 VbaModule.SourceCode의 쓰기가 지원됩니다."
type: docs
weight: 70
url: /ko/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

MPP 파일에서 기존 VBA 매크로 데이터를 업데이트할지 여부를 나타내는 값을 가져오거나 설정합니다. 현재 VbaModule.SourceCode의 기록이 지원됩니다.

```csharp
public bool WriteVba { get; set; }
```

## 예제

MPP 파일의 기존 VbaProject에 VBA 매크로를 추가/삭제하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

            var newModule = VbaModule.CreateProceduralModule("Module20");
            newModule.SourceCode = @"Sub TestMacro()
#If conUnicode Then
Dim p As Project
Set p = Application.ActiveProject
MsgBox ""This is a message from a new macro. Current project: "" & p.Name
#End If
End Sub

Private Sub Project_BeforePrint(ByVal pj As Project)

End Sub";
            project.VbaProject.Modules.Add(newModule);

            var moduleToDelete = project.VbaProject.Modules["EventCode"];
            project.VbaProject.Modules.Remove(moduleToDelete);

            project.Save(OutDir + "VbaProject.AddedModule.mpp", new MPPSaveOptions() { WriteVba = true });
```

### 또 보기

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


