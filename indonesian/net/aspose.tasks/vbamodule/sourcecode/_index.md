---
title: "VbaModule.SourceCode"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti VbaModule. Mendapatkan atau mengatur kode sumber modul VBA"
type: docs
weight: 50
url: /id/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

Mendapatkan atau mengatur kode sumber modul VBA

```csharp
public string SourceCode { get; set; }
```

## Contoh

Menampilkan cara membaca modul proyek VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

Menampilkan cara menambah/menghapus makro VBA ke/dari VbaProject yang ada dalam file MPP.

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

### Lihat Juga

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


