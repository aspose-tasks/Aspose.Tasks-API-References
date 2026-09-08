---
title: "MPPSaveOptions.WriteVba"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad MPPSaveOptions. Obtiene o establece un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. Actualmente se admite la escritura de VbaModule.SourceCode."
type: docs
weight: 70
url: /es/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Obtiene o establece un valor que indica si se deben actualizar los datos de macros VBA existentes en el archivo MPP. Actualmente se admite la escritura de VbaModule.SourceCode.

```csharp
public bool WriteVba { get; set; }
```

## Ejemplos

Muestra cómo agregar/eliminar macros VBA al/de la VbaProject existente en un archivo MPP.

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

### Ver también

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


