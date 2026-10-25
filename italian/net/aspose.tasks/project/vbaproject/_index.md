---
title: "Project.VbaProject"
second_title: "Riferimento API di Aspose.Tasks per .NET"
description: "Proprietà Project. Ottiene un'istanza della classe VbaProject"
type: docs
weight: 1010
url: /it/net/aspose.tasks/project/vbaproject/
---
## Project.VbaProject property

Ottiene un'istanza della classe `VbaProject`.

```csharp
public VbaProject VbaProject { get; }
```

## Esempi

Mostra come rimuovere le macro VBA dal file MPP.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");
project.Save(OutDir + "Vba.cleared.mpp", new MPPSaveOptions() { ClearVba = true });
```

Mostra come leggere le informazioni del progetto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("VbaProject.Name " + project.VbaProject.Name);
Console.WriteLine("VbaProject.Description " + project.VbaProject.Description);
Console.WriteLine("VbaProject.CompilationArguments" + project.VbaProject.CompilationArguments);
Console.WriteLine("VbaProject.HelpContextId" + project.VbaProject.HelpContextId);
Console.WriteLine("VbaProject.HelpFile" + project.VbaProject.HelpFile);
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

* class [VbaProject](../../vbaproject/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


