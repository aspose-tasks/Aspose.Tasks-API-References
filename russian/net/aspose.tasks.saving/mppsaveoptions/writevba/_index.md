---
title: "MPPSaveOptions.WriteVba"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство MPPSaveOptions. Возвращает или задает значение, указывающее, следует ли обновлять существующие данные макросов VBA в файле MPP. В настоящее время поддерживается запись VbaModule.SourceCode."
type: docs
weight: 70
url: /ru/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Получает или задает значение, указывающее, следует ли обновлять существующие данные макросов VBA в файле MPP. В настоящее время поддерживается запись VbaModule.SourceCode.

```csharp
public bool WriteVba { get; set; }
```

## Примеры

Показывает, как добавить/удалить макросы VBA в/из существующего VbaProject в файле MPP.

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

### См. также

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


