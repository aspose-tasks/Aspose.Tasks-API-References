---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks für .NET API-Referenz"
description: "MPPSaveOptions-Eigenschaft. Gibt einen Wert zurück oder legt ihn fest, der angibt, ob vorhandene VBA‑Makrodaten in einer MPP‑Datei aktualisiert werden sollen. Derzeit wird das Schreiben von VbaModule.SourceCode unterstützt."
type: docs
weight: 70
url: /de/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Gibt einen Wert zurück oder legt ihn fest, der angibt, ob vorhandene VBA‑Makrodaten in einer MPP‑Datei aktualisiert werden sollen. Derzeit wird das Schreiben von VbaModule.SourceCode unterstützt.

```csharp
public bool WriteVba { get; set; }
```

## Beispiele

Zeigt, wie man VBA-Makros zum/vom bestehenden VbaProject in einer MPP-Datei hinzufügt/entfernt.

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

### Siehe auch

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


