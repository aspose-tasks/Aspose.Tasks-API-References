---
title: Task
second_title: Aspose.Tasks لمرجع .NET API
description: يمثل مهمة في مشروع .
type: docs
weight: 2060
url: /ar/net/aspose.tasks/task/
---
## Task class

يمثل مهمة في مشروع .

```csharp
public class Task : IEquatable<Task>
```

## الخصائص

| اسم | وصف |
| --- | --- |
| [Assignments](../../aspose.tasks/task/assignments) { get; } | الحصول على مجموعة من تخصيصات الموارد لهذا الكائن. |
| [Baselines](../../aspose.tasks/task/baselines) { get; set; } | الحصول على مجموعة القيم الأساسية للمهمة أو تعيينها. |
| [Children](../../aspose.tasks/task/children) { get; } | الحصول على مجموعة مهام فرعية لهذا الكائن . كائن TaskCollection الذي يمثل المهام الفرعية. |
| [ExtendedAttributes](../../aspose.tasks/task/extendedattributes) { get; } | الحصول على كائن ExtendedAttributeCollection يحتوي على قيم سمة ممتدة. |
| [OutlineCodes](../../aspose.tasks/task/outlinecodes) { get; set; } | يحصل أو يحدد[`OutlineCodeCollection`](../outlinecodecollection) الكائن . |
| [ParentProject](../../aspose.tasks/task/parentproject) { get; } | الحصول على المشروع الأصلي لمهمة . |
| [ParentTask](../../aspose.tasks/task/parenttask) { get; } | الحصول على المهمة الرئيسية لمهمة . |
| [Predecessors](../../aspose.tasks/task/predecessors) { get; } | يحصل على أ[`TaskCollection`](../taskcollection) الكائن الذي يحتوي على جميع العناصر السابقة لكائن المهمة هذا. |
| [RecurringInfo](../../aspose.tasks/task/recurringinfo) { get; } | يحصل على مثيل[`RecurringTaskInfo`](../recurringtaskinfo) فئة للمهمة التي هي مهمة متكررة ؛ إذا لم تكن المهمة متكررة ، فستُرجع فارغة ؛  المعلومات الخاصة بمثيل[`RecurringTaskInfo`](../recurringtaskinfo) موجود بتنسيق ملف mpp فقط. |
| [SplitParts](../../aspose.tasks/task/splitparts) { get; } | الحصول على مجموعة SplitPart التي تمثل أجزاء مهمة. |
| [Successors](../../aspose.tasks/task/successors) { get; } | يحصل على أ[`TaskCollection`](../taskcollection) الكائن الذي يحتوي على جميع العناصر اللاحقة لكائن المهمة. |
| [TimephasedData](../../aspose.tasks/task/timephaseddata) { get; set; } | الحصول على كائن TimephasedDataCollection لهذه المهمة أو تعيينه. |

## طُرق

| اسم | وصف |
| --- | --- |
| [Clone](../../aspose.tasks/task/clone)() | إنشاء نسخة كاملة من مهمة بدون مهام فرعية. |
| [Delete](../../aspose.tasks/task/delete)() | حذف مهمة من مجموعة مهام المشروع الأصل وجميع مهامها. |
| override [Equals](../../aspose.tasks/task/equals#equals_1)(object) | إرجاع قيمة تشير إلى ما إذا كان هذا المثيل يساوي كائنًا محددًا. |
| [Equals](../../aspose.tasks/task/equals#equals)(Task) | إرجاع قيمة تشير إلى ما إذا كان هذا المثيل يساوي مهمة محددة. |
| [Get&lt;T&gt;](../../aspose.tasks/task/get)(Key&lt;T, TaskKey&gt;) | إرجاع القيمة التي تم تعيين الخاصية لها في هذه الحاوية. |
| override [GetHashCode](../../aspose.tasks/task/gethashcode)() | إرجاع قيمة رمز تجزئة لهذه المهمة. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata)(DateTime, DateTime) | عوائد[`TimephasedDataCollection`](../timephaseddatacollection) مع الكائن[`TimephasedData`](./timephaseddata) القيم ضمن تاريخي البدء والانتهاء المحددين. |
| [GetTimephasedData](../../aspose.tasks/task/gettimephaseddata#gettimephaseddata_1)(DateTime, DateTime, TimephasedDataType) | عوائد[`TimephasedDataCollection`](../timephaseddatacollection) مع الكائن[`TimephasedData`](./timephaseddata) القيم ضمن تواريخ البدء والانتهاء المحددة لنوع بيانات زمني محدد على مراحل. |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling_1)(int) | لنقل المهمة الحالية في نفس مستوى المخطط التفصيلي قبل مهمة بالمعرف المحدد. يحدد التواريخ المبكرة / المتأخرة) وحساب الحقول التابعة مثل فترات العمل وحقول العمل والتكلفة ومستويات المخطط التفصيلي) . إذا كان ParentProject.CalculationMode يدويًا ، فستحسب الطريقة فقط معرف المهمة ومستوى المخطط التفصيلي والأرقام التفصيلية تلقائيًا . إذا كان ParentProject. CalculationMode هو "تلقائي" الطريقة التي تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وتحسب فترات الركود ، وحقول العمل والتكلفة ، وإعادة حساب المعرفات ومستويات المخطط التفصيلي) . |
| [MoveToSibling](../../aspose.tasks/task/movetosibling#movetosibling)(Task) | ينقل المهمة الحالية في نفس مستوى المخطط التفصيلي قبل المهمة المحددة. إذا كان ParentProject.CalculationMode هو بلا مستخدم ، فيجب على المستخدم استدعاء Project.Recalculate () بعد استخدام هذه الطريقة (ستعيد جدولة جميع مهام المشروع (تواريخ البدء / الانتهاء ، وتعيين مبكرًا / التواريخ المتأخرة) وحساب الحقول التابعة مثل فترات السماح والعمل والتكلفة ومستويات المخطط التفصيلي) . إذا كان ParentProject.CalculationMode يدويًا ، فستحسب الطريقة فقط معرف المهمة ومستوى المخطط التفصيلي وأرقام المخطط التفصيلي تلقائيًا . إذا كان ParentProject.CalculationMode هو تلقائي تعيد الطريقة جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وتحسب فترات الركود ، وحقول العمل والتكلفة ، وإعادة حساب المعرفات ومستويات المخطط التفصيلي) . |
| [OutlineIndent](../../aspose.tasks/task/outlineindent)() | يضيف مسافة بادئة لمهمة في المخطط التفصيلي . |
| [OutlineOutdent](../../aspose.tasks/task/outlineoutdent)() | يقوم بترقية مهمة في المخطط التفصيلي . |
| [SelectAllChildTasks](../../aspose.tasks/task/selectallchildtasks)() | يقوم بتجميع كافة المهام الفرعية لهذه المهمة بشكل متكرر. |
| [Set&lt;T&gt;](../../aspose.tasks/task/set)(Key&lt;T, TaskKey&gt;, T) | تعيين الخاصية المحددة إلى القيمة المحددة في هذه الحاوية. |
| override [ToString](../../aspose.tasks/task/tostring)() | إرجاع تمثيل سلسلة قصيرة لمهمة . التفاصيل الدقيقة للتمثيل غير محددة وعرضة للتغيير. |

### ملاحظات

ال **مهمة** يمثل ظرفًا ذريًا واحدًا من العمل.

يمكن للمرء استخدامها **مهمة**لتخطيط مشروع عن طريق إنشاء المهام وتعيين الموارد المناسبة لها. يتم تنظيم المهام في المشروع كهيكل شجرة هرمية متجذرة ، مع مهمة جذرية وأشجار فرعية من المهام الفرعية.

لبناء شجرة من المهام ، يمكن للمرء استخدام مجموعة متخصصة[`TaskCollection`](../taskcollection) عن طريق الوصول[`RootTask`](../project/roottask) الملكية على سبيل المثال:

```csharp
Project project = new Project();

// إضافة مهام جديدة
Task task1 = project.RootTask.Children.Add(); // تمت إضافة مهمة رئيسية ذات اسم فارغ
Task childTask1 = task1.Children.Add("Child 1");
childTask1.Set(Tsk.Start, new DateTime(2020, 2, 12, 8, 0, 0))
childTask1.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask1.Set(Tsk.Finish, new DateTime(2020, 2, 12, 17, 0, 0));
Task childTask3 = task1.Children.Add("Child 3");
childTask3.Set(Tsk.Start, new DateTime(2020, 2, 13, 8, 0, 0))
childTask3.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask3.Set(Tsk.Finish, new DateTime(2020, 2, 13, 17, 0, 0));
Task childTask2 = task1.Children.Add("Child 2", 2); // يُدرج مهمة قبل التابع childTask3
childTask2.Set(Tsk.Start, new DateTime(2020, 2, 14, 8, 0, 0))
childTask2.Set(Tsk.Duration, project.GetDuration(8, TimeUnitType.Hour));
childTask2.Set(Tsk.Finish, new DateTime(2020, 2, 14, 17, 0, 0));

// حفظ المشروع بأحد التنسيقات المتاحة
project.Save("Filled project.xml", SaveFileFormat.MPP);
```

### أنظر أيضا

* مساحة الاسم [Aspose.Tasks](../../aspose.tasks)
* المجسم [Aspose.Tasks](../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->
