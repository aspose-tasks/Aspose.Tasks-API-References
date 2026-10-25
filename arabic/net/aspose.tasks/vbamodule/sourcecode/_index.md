---
title: "VbaModule.SourceCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية VbaModule. تحصل أو تعين شفرة المصدر لوحدة VBA."
type: docs
weight: 50
url: /ar/net/aspose.tasks/vbamodule/sourcecode/
---
## VbaModule.SourceCode property

يحصل أو يعيّن شفرة المصدر لوحدة VBA

```csharp
public string SourceCode { get; set; }
```

## الأمثلة

يوضح كيفية قراءة وحدات مشروع VBA.

```csharp
var project = new Project(DataDir + "VbaProject.mpp");

Console.WriteLine("Total Modules Count: " + project.VbaProject.Modules.Count);

foreach (var module in project.VbaProject.Modules)
{
    Console.WriteLine("Module Name: " + module.Name);
    Console.WriteLine("Source Code: " + module.SourceCode);
}
```

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


