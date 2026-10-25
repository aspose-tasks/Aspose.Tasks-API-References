---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET API リファレンス"
description: "MPPSaveOptions プロパティ。既存の VBA マクロ データを MPP ファイルで更新するかどうかを示す値を取得または設定します。現在、VbaModule.SourceCode の書き込みがサポートされています"
type: docs
weight: 70
url: /ja/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

既存の VBA マクロ データを MPP ファイルで更新するかどうかを示す値を取得または設定します。現在、VbaModule.SourceCode の書き込みがサポートされています。

```csharp
public bool WriteVba { get; set; }
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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


