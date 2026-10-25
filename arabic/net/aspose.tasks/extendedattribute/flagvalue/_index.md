---
title: "ExtendedAttribute.FlagValue"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "خاصية ExtendedAttribute. تحصل أو تعيّن قيمة تشير إلى ما إذا كان العلم مُعيّنًا لخاصية من نوع Flag."
type: docs
weight: 50
url: /ar/net/aspose.tasks/extendedattribute/flagvalue/
---
## ExtendedAttribute.FlagValue property

يحصل أو يعيّن قيمة تشير إلى ما إذا كان العلم مُعيّنًا للصفة ذات النوع 'Flag'.

```csharp
public bool FlagValue { get; set; }
```

### استثناءات

| استثناء | شرط |
| --- | --- |
| InvalidOperationException | يُرمى إذا لم يتم تهيئة خاصية [`AttributeDefinition`](../attributedefinition/) أو إذا لم تكن الخاصية الحالية من نوع علم. |

## الأمثلة

يوضح كيفية إنشاء خاصية موسعة منطقية.

```csharp
var project = new Project();

// إنشاء تعريف سمة موسعة جديدة للمهمة
var definition = ExtendedAttributeDefinition.CreateTaskDefinition(CustomFieldType.Flag, ExtendedAttributeTask.Flag1, "Is Finished");

// أضف صيغة إلى الخاصية.
definition.Formula = "[% Complete] = 100";

project.ExtendedAttributes.Add(definition);

var finished = project.RootTask.Children.Add("Task");
finished.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));
finished.Set(Tsk.ActualDuration, project.GetDuration(1, TimeUnitType.Day));
finished.Set(Tsk.ActualFinish, new DateTime(2020, 4, 21, 17, 0, 0));
finished.Set(Tsk.PercentComplete, 100);

var running = project.RootTask.Children.Add("Task");
running.Set(Tsk.Start, new DateTime(2020, 4, 21, 8, 0, 0));
running.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
running.Set(Tsk.Finish, new DateTime(2020, 4, 21, 17, 0, 0));
running.Set(Tsk.ActualStart, new DateTime(2020, 4, 21, 8, 0, 0));

Console.WriteLine(running.Get(Tsk.PercentComplete));
// إنشاء خاصية موسعة
var runningFlagAttribute = definition.CreateExtendedAttribute();
var finishedFlagAttribute = definition.CreateExtendedAttribute();
running.ExtendedAttributes.Add(runningFlagAttribute);
finished.ExtendedAttributes.Add(finishedFlagAttribute);

Console.WriteLine("Alias: {0}\n", definition.Alias);
Console.WriteLine("(Finished Task) Field Id: " + finishedFlagAttribute.FieldId);
Console.WriteLine("(Finished Task) Value: {0}\n", finishedFlagAttribute.FlagValue);
Console.WriteLine("(Running Task) Field Id: " + runningFlagAttribute.FieldId);
Console.WriteLine("(Running Task) Value: " + runningFlagAttribute.FlagValue);
```

### انظر أيضًا

* class [ExtendedAttribute](../)
* namespace [Aspose.Tasks](../../extendedattribute/)
* assembly [Aspose.Tasks](../../../)


