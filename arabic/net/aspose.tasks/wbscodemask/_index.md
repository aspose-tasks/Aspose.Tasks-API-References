---
title: "الفئة WBSCodeMask"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "الفئة Aspose.Tasks.WBSCodeMask. تمثل قناع رمز WBS"
type: docs
weight: 3500
url: /ar/net/aspose.tasks/wbscodemask/
---
## WBSCodeMask class

يمثل قناع رمز WBS.

```csharp
public class WBSCodeMask
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WBSCodeMask](wbscodemask/)() | يُهيئ نسخة جديدة من الفئة `WBSCodeMask`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Length](../../aspose.tasks/wbscodemask/length/) { get; set; } | يحصل أو يعيّن عدد الأحرف في سلسلة الرمز. |
| [Level](../../aspose.tasks/wbscodemask/level/) { get; } | يحصل على مستوى القناع. |
| [Separator](../../aspose.tasks/wbscodemask/separator/) { get; set; } | يحصل أو يضبط الفاصل لسلسلة الرمز. القيمة الافتراضية هي النقطة. |
| [Sequence](../../aspose.tasks/wbscodemask/sequence/) { get; set; } | يحصل أو يضبط نوع الحرف لسلسلة الرمز. |

## الأمثلة

يعرض كيفية إنشاء أقنعة رموز WBS.

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

var task = project.RootTask.Children.Add("Task 1");
task.Children.Add("Task 2");

project.Recalculate();

Console.WriteLine("Number of WBS masks: " + project.WBSCodeDefinition.CodeMaskCollection.Count);
var i = 0;
foreach (var cm in project.WBSCodeDefinition.CodeMaskCollection)
{
    Console.WriteLine("WBS Mask #{0}: Level->{1}", ++i, cm.Level);
}

project.Save(OutDir + @"AddWBSCodes_out.xml", SaveFileFormat.Xml);
```

### انظر أيضًا

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


