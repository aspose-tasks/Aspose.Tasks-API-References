---
title: "VbaModule.SourceCode"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "VbaModule eigenschap. Haalt of stelt de broncode van de VBA-module in"
type: docs
weight: 50
url: /nl/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

Haalt de broncode van de VBA-module op of stelt deze in

```csharp
public string SourceCode { get; set; }
```

## Voorbeelden

Toont hoe modules van een VBA-project gelezen kunnen worden.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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


