---
title: "Task.MoveToSibling"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Task. تنقل المهمة الحالية في نفس مستوى المخطط قبل المهمة المحددة. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate بعد استخدام هذه الطريقة. سيعيد جدولة جميع تواريخ بدء/إنهاء مهام المشروع، يحدد تواريخ مبكرة/متأخرة، ويحساب الحقول التابعة مثل الفترات المتبقية والعمل وتكاليف الحقول ومستويات المخطط. إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة ومستوى المخطط وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا، تواريخ البدء/الإنهاء، تحدد تواريخ مبكرة/متأخرة، تحسب الفترات المتبقية والعمل وتكاليف الحقول، تعيد حساب المعرفات ومستويات المخطط"
type: docs
weight: 1370
url: /ar/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

ينقل المهمة الحالية في نفس مستوى المخطط (Outline Level) قبل المهمة المحددة. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحساب الحقول التابعة مثل الفجوات، العمل وتكاليف الحقول، مستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، مستوى المخطط وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، العمل وتكاليف الحقول، يعيد حساب المعرفات ومستويات المخطط).

```csharp
public void MoveToSibling(Task beforeTask)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| beforeTask | مهمة | المهمة التي سيُدرج قبلها المهمة الحالية. |

## الأمثلة

يعرض كيفية نقل المهمة تحت نفس الأصل.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// نقل المهام ذات المعرف 5 قبل المهمة ذات المعرف 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// أو
// نقل المهمة إلى نهاية المجموعة
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

ينقل المهمة الحالية في نفس مستوى المخطط (Outline Level) قبل مهمة ذات المعرف المحدد (Id). إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحساب الحقول التابعة مثل الفجوات، العمل وتكاليف الحقول، مستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، مستوى المخطط وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، العمل وتكاليف الحقول، يعيد حساب المعرفات ومستويات المخطط).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| beforeTaskId | Int32 | معرف ([`Id`](../../tsk/id/)) للمهمة التي سيُدرج قبلها المهمة الحالية. |

## الأمثلة

يعرض كيفية نقل المهمة تحت نفس الأصل باستخدام معرف المهمة.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// نقل المهام ذات المعرف 5 قبل المهمة ذات المعرف 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// أو
// نقل المهمة إلى نهاية المجموعة
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### انظر أيضًا

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


