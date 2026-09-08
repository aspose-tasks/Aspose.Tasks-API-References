---
title: "VbaModule.CreateProceduralModule"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "VbaModule メソッド。VbaModuleType.ProceduralModule タイプの VbaModule のインスタンスを作成します"
type: docs
weight: 20
url: /ja/net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

VbaModuleType.ProceduralModule タイプの [`VbaModule`](../) のインスタンスを作成します。

```csharp
public static VbaModule CreateProceduralModule(string name)
```

## 例

MPP ファイル内の既存 VbaProject に VBA マクロを追加/削除する方法を示します。

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

### 関連項目

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


