---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModule 属性。获取或设置 VBA 模块的源代码"
type: docs
weight: 50
url: /zh/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

获取或设置 VBA 模块的源代码

```csharp
public string SourceCode { get; set; }
```

## 示例

展示如何读取 VBA 项目的模块。

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

展示如何在 MPP 文件中对现有 VbaProject 添加/删除 VBA 宏。

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

### 另见

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


