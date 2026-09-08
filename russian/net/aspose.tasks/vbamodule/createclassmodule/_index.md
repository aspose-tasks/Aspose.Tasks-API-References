---
title: "VbaModule.CreateClassModule"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Метод VbaModule. Создаёт экземпляр VbaModule типа VbaModuleType.ClassModule"
type: docs
weight: 10
url: /ru/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

Создаёт экземпляр [`VbaModule`](../) типа VbaModuleType.ClassModule.

```csharp
public static VbaModule CreateClassModule(string name)
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


