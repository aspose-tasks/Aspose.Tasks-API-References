---
title: MoveToSibling
second_title: Aspose.Tasks لمرجع .NET API
description: ينقل المهمة الحالية في نفس مستوى المخطط التفصيلي قبل المهمة المحددة. إذا كان ParentProject.CalculationMode هو بلا مستخدم  فيجب على المستخدم استدعاء Project.Recalculate  بعد استخدام هذه الطريقة ستعيد جدولة جميع مهام المشروع تواريخ البدء / الانتهاء  وتعيين مبكرًا / التواريخ المتأخرة وحساب الحقول التابعة مثل فترات السماح والعمل والتكلفة ومستويات المخطط التفصيلي . إذا كان ParentProject.CalculationMode يدويًا  فستحسب الطريقة فقط معرف المهمة ومستوى المخطط التفصيلي وأرقام المخطط التفصيلي تلقائيًا . إذا كان ParentProject.CalculationMode هو تلقائي تعيد الطريقة جدولة جميع مهام المشروع تلقائيًا تواريخ البدء / الانتهاء  وتعيين التواريخ المبكرة / المتأخرة  وتحسب فترات الركود  وحقول العمل والتكلفة  وإعادة حساب المعرفات ومستويات المخطط التفصيلي .
type: docs
weight: 190
url: /ar/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

ينقل المهمة الحالية في نفس مستوى المخطط التفصيلي قبل المهمة المحددة. إذا كان ParentProject.CalculationMode هو بلا مستخدم ، فيجب على المستخدم استدعاء Project.Recalculate () بعد استخدام هذه الطريقة (ستعيد جدولة جميع مهام المشروع (تواريخ البدء / الانتهاء ، وتعيين مبكرًا / التواريخ المتأخرة) وحساب الحقول التابعة مثل فترات السماح والعمل والتكلفة ومستويات المخطط التفصيلي) . إذا كان ParentProject.CalculationMode يدويًا ، فستحسب الطريقة فقط معرف المهمة ومستوى المخطط التفصيلي وأرقام المخطط التفصيلي تلقائيًا . إذا كان ParentProject.CalculationMode هو تلقائي تعيد الطريقة جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وتحسب فترات الركود ، وحقول العمل والتكلفة ، وإعادة حساب المعرفات ومستويات المخطط التفصيلي) .

```csharp
public void MoveToSibling(Task beforeTask)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| beforeTask | Task | المهمة التي سيتم إدراج المهمة الحالية قبلها. |

### أنظر أيضا

* class [Task](../../task)
* مساحة الاسم [Aspose.Tasks](../../task)
* المجسم [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

لنقل المهمة الحالية في نفس مستوى المخطط التفصيلي قبل مهمة بالمعرف المحدد. يحدد التواريخ المبكرة / المتأخرة) وحساب الحقول التابعة مثل فترات العمل وحقول العمل والتكلفة ومستويات المخطط التفصيلي) . إذا كان ParentProject.CalculationMode يدويًا ، فستحسب الطريقة فقط معرف المهمة ومستوى المخطط التفصيلي والأرقام التفصيلية تلقائيًا . إذا كان ParentProject. CalculationMode هو "تلقائي" الطريقة التي تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة ، وتحسب فترات الركود ، وحقول العمل والتكلفة ، وإعادة حساب المعرفات ومستويات المخطط التفصيلي) .

```csharp
public void MoveToSibling(int beforeTaskId)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| beforeTaskId | Int32 | هوية شخصية ([`Id`](../../tsk/id)) لمهمة سيتم إدراج المهمة الحالية قبلها. |

### أنظر أيضا

* class [Task](../../task)
* مساحة الاسم [Aspose.Tasks](../../task)
* المجسم [Aspose.Tasks](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Tasks.dll -->