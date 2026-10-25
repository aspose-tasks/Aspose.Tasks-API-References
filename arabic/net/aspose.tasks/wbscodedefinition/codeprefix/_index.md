---
title: "WBSCodeDefinition.CodePrefix"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WBSCodeDefinition. تحصل أو تعين بادئة رمز المشروع"
type: docs
weight: 30
url: /ar/net/aspose.tasks/wbscodedefinition/codeprefix/
---
## WBSCodeDefinition.CodePrefix property

يحصل أو يعيّن بادئة رمز المشروع.

```csharp
public string CodePrefix { get; set; }
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


