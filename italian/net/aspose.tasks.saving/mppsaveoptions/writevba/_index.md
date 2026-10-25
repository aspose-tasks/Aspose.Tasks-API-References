---
title: "MPPSaveOptions.WriteVba"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà MPPSaveOptions. Ottiene o imposta un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. Attualmente è supportata la scrittura di VbaModule.SourceCode."
type: docs
weight: 70
url: /it/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Ottiene o imposta un valore che indica se aggiornare i dati delle macro VBA esistenti nel file MPP. Attualmente è supportata la scrittura di VbaModule.SourceCode.

```csharp
public bool WriteVba { get; set; }
```

## Esempi

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


