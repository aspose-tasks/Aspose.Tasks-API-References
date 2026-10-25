---
title: "VbaModuleCollection.Remove"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Método VbaModuleCollection."
type: docs
weight: 90
url: /es/net/aspose.tasks/vbamodulecollection/remove/
---
## VbaModuleCollection.Remove method

```csharp
public bool Remove(VbaModule item)
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

* class [VbaModule](../../vbamodule/)
* class [VbaModuleCollection](../)
* namespace [Aspose.Tasks](../../vbamodulecollection/)
* assembly [Aspose.Tasks](../../../)


