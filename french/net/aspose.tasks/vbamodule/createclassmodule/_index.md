---
title: "VbaModule.CreateClassModule"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Méthode VbaModule. Crée une instance de VbaModule avec le type VbaModuleType.ClassModule"
type: docs
weight: 10
url: /fr/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

Crée une instance de [`VbaModule`](../) avec le type VbaModuleType.ClassModule.

```csharp
public static VbaModule CreateClassModule(string name)
```

## Exemples

Montre comment ajouter/supprimer des macros VBA dans/à partir du VbaProject existant dans un fichier MPP.

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

### Voir aussi

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


