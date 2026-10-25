---
title: "Project.WBSCodeDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية Project. تحصل أو تعين WBS Code Definition للمشروع"
type: docs
weight: 1030
url: /ar/net/aspose.tasks/project/wbscodedefinition/
---
## Project.WBSCodeDefinition property

يحصل أو يضبط تعريف رمز WBS للمشروع.

```csharp
public WBSCodeDefinition WBSCodeDefinition { get; set; }
```

## الأمثلة

يوضح كيفية إضافة رموز WBS.

```csharp
var project = new Project
{
    WBSCodeDefinition = new WBSCodeDefinition()
};
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask
{
    Length = 2,
    Separator = "-",
    Sequence = WBSSequence.OrderedNumbers
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask
{
    Length = 1,
    Separator = "-",
    Sequence = WBSSequence.OrderedUppercaseLetters
};
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [WBSCodeDefinition](../../wbscodedefinition/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


