---
title: "VbaModule.SourceCode"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaModule. Obtiene o establece el código fuente del módulo VBA"
type: docs
weight: 50
url: /es/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

Obtiene o establece el código fuente del módulo VBA

```csharp
public string SourceCode { get; set; }
```

## Ejemplos

Muestra cómo leer los módulos del proyecto VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


