---
title: "VbaModule.CreateClassModule"
second_title: "Aspose.Tasks for .NET API 参考"
description: "VbaModule 方法。创建一个 VbaModule 实例，类型为 VbaModuleType.ClassModule"
type: docs
weight: 10
url: /zh/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

创建一个 [`VbaModule`](../) 实例，类型为 VbaModuleType.ClassModule。

```csharp
public static VbaModule CreateClassModule(string name)
```

## 示例

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


