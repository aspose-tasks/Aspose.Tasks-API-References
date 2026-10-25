---
title: "MPPSaveOptions.WriteVba"
second_title: "Référence de l'API Aspose.Tasks for .NET"
description: "Propriété MPPSaveOptions. Obtient ou définit une valeur indiquant s'il faut mettre à jour les données des macros VBA existantes dans le fichier MPP. L'écriture de VbaModule.SourceCode est actuellement prise en charge."
type: docs
weight: 70
url: /fr/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Obtient ou définit une valeur indiquant s'il faut mettre à jour les données de macros VBA existantes dans le fichier MPP. L'écriture de VbaModule.SourceCode est actuellement prise en charge.

```csharp
public bool WriteVba { get; set; }
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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


