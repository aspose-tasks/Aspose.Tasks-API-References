---
title: "VbaProject.Modules"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaProject 속성. VbaModuleCollection 컬렉션을 가져옵니다"
type: docs
weight: 50
url: /ko/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

[`VbaModuleCollection`](../../vbamodulecollection/) 컬렉션을 가져옵니다

```csharp
public VbaModuleCollection Modules { get; }
```

## 예제

프로젝트의 VBS 모듈을 반복하는 방법을 보여줍니다.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


