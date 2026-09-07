---
title: "VbaProject.Modules"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "VbaProject ιδιότητα. Λαμβάνει μια συλλογή του VbaModuleCollection"
type: docs
weight: 50
url: /el/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

Λαμβάνει μια συλλογή του [`VbaModuleCollection`](../../vbamodulecollection/)

```csharp
public VbaModuleCollection Modules { get; }
```

## Παραδείγματα

Δείχνει πώς να επαναλάβετε τις μονάδες VBS του έργου.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


