---
title: "VbaProject.Modules"
second_title: "Referencia de API de Aspose.Tasks para .NET"
description: "Propiedad VbaProject. Obtiene una colección de VbaModuleCollection"
type: docs
weight: 50
url: /es/net/aspose.tasks/vbaproject/modules/
---
## VbaProject.Modules property

Obtiene una colección de [`VbaModuleCollection`](../../vbamodulecollection/)

```csharp
public VbaModuleCollection Modules { get; }
```

## Ejemplos

Muestra cómo iterar sobre los módulos VBS del proyecto.

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

* class [VbaModuleCollection](../../vbamodulecollection/)
* class [VbaProject](../)
* namespace [Aspose.Tasks](../../vbaproject/)
* assembly [Aspose.Tasks](../../../)


