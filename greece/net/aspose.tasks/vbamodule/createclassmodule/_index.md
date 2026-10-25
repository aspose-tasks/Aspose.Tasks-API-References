---
title: "VbaModule.CreateClassModule"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος VbaModule. Δημιουργεί μια παρουσία του VbaModule με τύπο VbaModuleType.ClassModule"
type: docs
weight: 10
url: /el/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

Δημιουργεί μια παρουσία του [`VbaModule`](../) με τύπο VbaModuleType.ClassModule.

```csharp
public static VbaModule CreateClassModule(string name)
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε/διαγράψετε μακροεντολές VBA σε/από το υπάρχον VbaProject σε αρχείο MPP.

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

### Δείτε επίσης

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


