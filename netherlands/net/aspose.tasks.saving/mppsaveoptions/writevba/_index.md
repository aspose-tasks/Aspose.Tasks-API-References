---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET API-referentie"
description: "MPPSaveOptions‑eigenschap. Haalt een waarde op of stelt deze in die aangeeft of bestaande VBA‑macro‑gegevens in het MPP‑bestand moeten worden bijgewerkt. Momenteel wordt het schrijven van VbaModule.SourceCode ondersteund."
type: docs
weight: 70
url: /nl/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Haalt op of stelt een waarde in die aangeeft of bestaande VBA-macrogegevens in het MPP‑bestand moeten worden bijgewerkt. Momenteel wordt het schrijven van VbaModule.SourceCode ondersteund.

```csharp
public bool WriteVba { get; set; }
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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


