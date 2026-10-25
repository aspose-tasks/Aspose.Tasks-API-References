---
title: "VbaProject.Modules"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "VbaProject property. Ottiene una raccolta di VbaModuleCollection"
type: docs
weight: 50
url: /it/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

Ottiene una raccolta di [`VbaModuleCollection`](../../vbamodulecollection/)

```csharp
public VbaModuleCollection Modules { get; }
```

## Esempi

Mostra come iterare sui moduli VBS del progetto.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

Mostra come aggiungere/rimuovere le macro VBA al/dal VbaProject esistente nel file MPP.

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

### Vedi anche

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


