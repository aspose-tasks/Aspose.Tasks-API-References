---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET API 参考"
description: "MPPSaveOptions 属性。获取或设置一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。当前支持写入 VbaModule.SourceCode。"
type: docs
weight: 70
url: /zh/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

获取或设置一个值，指示是否在 MPP 文件中更新现有的 VBA 宏数据。当前支持写入 VbaModule.SourceCode。

```csharp
public bool WriteVba { get; set; }
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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


