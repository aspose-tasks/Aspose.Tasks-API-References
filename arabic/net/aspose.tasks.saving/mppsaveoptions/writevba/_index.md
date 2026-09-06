---
title: "MPPSaveOptions.WriteVba"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية MPPSaveOptions. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. كتابة VbaModule.SourceCode مدعومة حاليًا."
type: docs
weight: 70
url: /ar/net/aspose.tasks.saving/mppsaveoptions/writevba/
---
## MPPSaveOptions.WriteVba property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب تحديث بيانات ماكرو VBA الموجودة في ملف MPP. حاليًا يتم دعم كتابة VbaModule.SourceCode.

```csharp
public bool WriteVba { get; set; }
```

## الأمثلة

يظهر كيفية إضافة/حذف ماكرو VBA إلى/من VbaProject الموجود في ملف MPP.

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

### انظر أيضًا

* class [MPPSaveOptions](../)
* namespace [Aspose.Tasks.Saving](../../mppsaveoptions/)
* assembly [Aspose.Tasks](../../../)


