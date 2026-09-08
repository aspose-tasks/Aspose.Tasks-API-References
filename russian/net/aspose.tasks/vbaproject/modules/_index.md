---
title: "VbaProject.Modules"
second_title: "Справочник API Aspose.Tasks for .NET"
description: "Свойство VbaProject. Получает коллекцию VbaModuleCollection"
type: docs
weight: 50
url: /ru/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

Получает коллекцию [`VbaModuleCollection`](../../vbamodulecollection/)

```csharp
public VbaModuleCollection Modules { get; }
```

## Примеры

Показывает, как перебрать VBS‑модули проекта.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


