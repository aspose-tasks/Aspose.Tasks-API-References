---
title: "WBSCodeDefinition.CodeMaskCollection"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية WBSCodeDefinition. تحصل على مجموعة كائنات WBSCodeMask"
type: docs
weight: 20
url: /ar/net/aspose.tasks/wbscodedefinition/codemaskcollection/
---
## WBSCodeDefinition.CodeMaskCollection property

يحصل على مجموعة كائنات WBSCodeMask.

```csharp
public WBSCodeMaskCollection CodeMaskCollection { get; }
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

* class [WBSCodeMaskCollection](../../wbscodemaskcollection/)
* class [WBSCodeDefinition](../)
* namespace [Aspose.Tasks](../../wbscodedefinition/)
* assembly [Aspose.Tasks](../../../)


