---
title: "Enum WBSSequence"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "Aspose.Tasks.WBSSequence enum. يحدد التسلسل لـ WBSCodeMask"
type: docs
weight: 3520
url: /ar/net/aspose.tasks/wbssequence/
---
## WBSSequence enumeration

يحدد التسلسل لـ WBSCodeMask

```csharp
public enum WBSSequence
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| OrderedNumbers | `0` | يشير إلى تسلسل أرقام WBS. |
| OrderedUppercaseLetters | `1` | يشير إلى تسلسل أحرف WBS الكبيرة. |
| OrderedLowercaseLetters | `2` | يشير إلى تسلسل أحرف WBS الصغيرة. |
| UnorderedCharacters | `3` | يشير إلى تسلسل أحرف WBS غير المرتبة. |

## الأمثلة

يوضح كيفية ضبط تسلسلات WBS.

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


