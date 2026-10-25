---
title: "MPPSaveOptions.WriteVba"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Ιδιότητα MPPSaveOptions. Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα ενημερωθούν τα υπάρχοντα δεδομένα μακροεντολών VBA στο αρχείο MPP. Αυτή τη στιγμή υποστηρίζεται η εγγραφή του VbaModule.SourceCode."
type: docs
weight: 70
url: /el/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

Λαμβάνει ή ορίζει μια τιμή που υποδεικνύει εάν θα ενημερωθούν τα υπάρχοντα δεδομένα μακροεντολών VBA στο αρχείο MPP. Προς το παρόν υποστηρίζεται η εγγραφή του VbaModule.SourceCode.

```csharp
public bool WriteVba { get; set; }
```

## Παραδείγματα

Δείχνει πώς να προσθέσετε/διαγράψετε μακροεντολές VBA σε/από το υπάρχον VbaProject σε αρχείο MPP.

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

### Δείτε επίσης

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


