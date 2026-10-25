---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα VbaModule. Λαμβάνει ή ορίζει έναν κώδικα πηγής της μονάδας VBA"
type: docs
weight: 50
url: /el/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

Λαμβάνει ή ορίζει τον πηγαίο κώδικα της μονάδας VBA

```csharp
public string SourceCode { get; set; }
```

## Παραδείγματα

Δείχνει πώς να διαβάσετε τις μονάδες του έργου VBA.

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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


