---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API 참조"
description: "VbaModule 속성. VBA 모듈의 소스 코드를 가져오거나 설정합니다."
type: docs
weight: 50
url: /ko/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

VBA 모듈의 소스 코드를 가져오거나 설정합니다.

```csharp
public string SourceCode { get; set; }
```

## 예제

VBA 프로젝트의 모듈을 읽는 방법을 보여줍니다.

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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


