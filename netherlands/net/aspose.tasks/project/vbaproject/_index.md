---
title: "Project.VbaProject"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "Projecteigenschap. Haalt een instantie van de VbaProject‑klasse op."
type: docs
weight: 1010
url: /nl/net/aspose.tasks/project/vbaproject/
---
## Project.VbaProject property

Haalt een instantie van de `VbaProject`‑klasse op.

```csharp
public VbaProject VbaProject { get; }
```

## Voorbeelden

Toont hoe u VBA‑macro's uit een MPP‑bestand kunt verwijderen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

Toont hoe u VBA‑projectinformatie kunt lezen.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
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

* class [VbaProject](../../vbaproject/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


