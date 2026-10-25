---
title: "VbaModule.CreateProceduralModule"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "VbaModule Methode. Erstellt eine Instanz von VbaModule mit dem Typ VbaModuleType.ProceduralModule"
type: docs
weight: 20
url: /de/net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

Erstellt eine Instanz von [`VbaModule`](../) mit dem Typ VbaModuleType.ProceduralModule.

```csharp
public static VbaModule CreateProceduralModule(string name)
```

## Beispiele

Zeigt, wie man VBA-Makros zum/vom bestehenden VbaProject in einer MPP-Datei hinzufügt/entfernt.

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

### Siehe auch

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


