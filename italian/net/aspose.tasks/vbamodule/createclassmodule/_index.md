---
title: "VbaModule.CreateClassModule"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Metodo VbaModule. Crea un'istanza di VbaModule con il tipo VbaModuleType.ClassModule"
type: docs
weight: 10
url: /it/net/aspose.tasks/vbamodule/createclassmodule/
---
## VbaModule.CreateClassModule method

Crea un'istanza di [`VbaModule`](../) con il tipo VbaModuleType.ClassModule.

```csharp
public static VbaModule CreateClassModule(string name)
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


