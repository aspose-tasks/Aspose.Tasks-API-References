---
title: "MPPSaveOptions.WriteVba"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti MPPSaveOptions. Mendapatkan atau mengatur nilai yang menunjukkan apakah data makro VBA yang ada harus diperbarui dalam file MPP. Saat ini penulisan VbaModule.SourceCode didukung."
type: docs
weight: 70
url: /id/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Mendapatkan atau mengatur nilai yang menunjukkan apakah akan memperbarui data makro VBA yang ada dalam file MPP. Saat ini penulisan VbaModule.SourceCode didukung.

```csharp
public bool WriteVba { get; set; }
```

## Contoh

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

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


