---
title: "VbaModule.CreateProceduralModule"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة VbaModule. تُنشئ نسخة من VbaModule بنوع VbaModuleType.ProceduralModule."
type: docs
weight: 20
url: /ar/net/aspose.tasks/vbamodule/createproceduralmodule/
---
## VbaModule.CreateProceduralModule method

ينشئ نسخة من [`VbaModule`](../) بنوع VbaModuleType.ProceduralModule.

```csharp
public static VbaModule CreateProceduralModule(string name)
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

* class [VbaModule](../)
* namespace [Aspose.Tasks](../../vbamodule/)
* assembly [Aspose.Tasks](../../../)


