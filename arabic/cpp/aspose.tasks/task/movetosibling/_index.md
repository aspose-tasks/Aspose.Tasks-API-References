---
title: "Aspose::Tasks::Task::MoveToSibling method"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks لـ C++"
description: "ينقل المهمة الحالية في نفس مستوى المخطط قبل المهمة المحددة."
type: docs
weight: 1370
url: /ar/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

ينقل المهمة الحالية في نفس مستوى المخطط قبل المهمة المحددة. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحسب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، ومستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرّف المهمة، مستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، تحدد تواريخ مبكرة/متأخرة، تحسب الفجوات، والعمل، وتكاليف الحقول، وتعيد حساب المعرفات ومستويات المخطط).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| معامل | الوصف |
| --- | --- |
| beforeTask | المهمة التي سيُدرج قبلها المهمة الحالية. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

ينقل المهمة الحالية في نفس مستوى المخطط قبل مهمة ذات المعرف المحدد. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (سيعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة) ويحساب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، ومستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، مستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، يحدد تواريخ مبكرة/متأخرة، يحسب الفجوات، والعمل، وتكاليف الحقول، ويعيد حساب المعرفات ومستويات المخطط).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| معامل | الوصف |
| --- | --- |
| beforeTaskId | معرف ( Tsk::Id ) للمهمة التي سيُدرج قبلها المهمة الحالية. |

