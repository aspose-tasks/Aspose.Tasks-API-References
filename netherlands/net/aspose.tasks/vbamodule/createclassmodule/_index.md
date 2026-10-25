---
title: "VbaModule.CreateClassModule"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModule methode. Maakt een instantie van VbaModule met type VbaModuleType.ClassModule"
type: docs
weight: 10
url: /nl/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

Maakt een instantie van [`VbaModule`](../) met type VbaModuleType.ClassModule.

```csharp
public static VbaModule CreateClassModule(string name)
```

## Voorbeelden

Toont hoe u VBA‑macro's kunt toevoegen/verwijderen aan/van het bestaande VbaProject in een MPP‑bestand.

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

### Zie ook

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


