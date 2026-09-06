---
title: "الفئة WBSCodeDefinition"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "فئة Aspose.Tasks.WBSCodeDefinition. تمثل تعريف رمز WBS."
type: docs
weight: 3490
url: /ar/net/aspose.tasks/wbscodedefinition/
---
## WBSCodeDefinition class

يمثل تعريف رمز WBS.

```csharp
public class WBSCodeDefinition
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [WBSCodeDefinition](wbscodedefinition/)() | ينشئ مثلاً جديداً من الفئة `WBSCodeDefinition`. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [CodeMaskCollection](../../aspose.tasks/wbscodedefinition/codemaskcollection/) { get; } | يحصل على مجموعة كائنات WBSCodeMask. |
| [CodePrefix](../../aspose.tasks/wbscodedefinition/codeprefix/) { get; set; } | يحصل أو يعيّن بادئة رمز المشروع. |
| [GenerateWBSCode](../../aspose.tasks/wbscodedefinition/generatewbscode/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب توليد رمز WBS للمهمة الجديدة. |
| [VerifyUniqueness](../../aspose.tasks/wbscodedefinition/verifyuniqueness/) { get; set; } | يحصل أو يعيّن قيمة تشير إلى ما إذا كان يجب التحقق من تفرد رموز WBS الجديدة. |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


