---
title: "VbaModule.SourceCode"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété VbaModule. Obtient ou définit le code source du module VBA"
type: docs
weight: 50
url: /fr/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

Obtient ou définit le code source du module VBA.

```csharp
public string SourceCode { get; set; }
```

## Exemples

Montre comment lire les modules du projet VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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


