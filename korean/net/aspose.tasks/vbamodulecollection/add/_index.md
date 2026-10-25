---
title: "VbaModuleCollection.Add"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModuleCollection 메서드."
type: docs
weight: 40
url: /ko/net/aspose.tasks/vbamodulecollection/add/
---
## VbaModuleCollection.Add method

```csharp
public void Add(VbaModule item)
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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


