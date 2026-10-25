---
title: "WBSCodeDefinition.GenerateWBSCode"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WBSCodeDefinition. تحصل أو تعين قيمة تشير إلى ما إذا كان يجب توليد رمز WBS للمهمة الجديدة"
type: docs
weight: 40
url: /ar/net/aspose.tasks/wbscodedefinition/generatewbscode/
---
## WBSCodeDefinition.GenerateWBSCode property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب توليد رمز WBS للمهمة الجديدة.

```csharp
public bool GenerateWBSCode { get; set; }
```

## الأمثلة

يوضح كيفية إضافة أقنعة رمز WBS.

```csharp
var project = new Project();

project.WBSCodeDefinition = new WBSCodeDefinition();
project.WBSCodeDefinition.GenerateWBSCode = true;
project.WBSCodeDefinition.VerifyUniqueness = true;
project.WBSCodeDefinition.CodePrefix = "CRS-";

var mask = new WBSCodeMask();
mask.Length = 2;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedNumbers;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

mask = new WBSCodeMask();
mask.Length = 1;
mask.Separator = "-";
mask.Sequence = WBSSequence.OrderedUppercaseLetters;
project.WBSCodeDefinition.CodeMaskCollection.Add(mask);

var tsk = project.RootTask.Children.Add("Task 1");
tsk.Children.Add("Task 2");

project.Recalculate();

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


