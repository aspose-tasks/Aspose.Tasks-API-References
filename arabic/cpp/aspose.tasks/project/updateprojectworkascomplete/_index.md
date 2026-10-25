---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete طريقة"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks لـ C++"
description: "يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للمشروع بأكمله."
type: docs
weight: 2080
url: /ar/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

يحدّث جميع الأعمال كمنجزة حتى تاريخ محدد للمشروع بأكمله.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| معامل | الوصف |
| --- | --- |
| completeThrough | التاريخ لتحديث العمل على أنه مكتمل حتى. |
| setZeroOrHundredPercentCompleteOnly | إذا تم تعيينه إلى true، يتم تحديث تلك المهام فقط إلى 100٪ مكتملة إذا كان تاريخ الانتهاء قبل تاريخ الإكمال المحدد. وإلا، يتم حساب قيمة النسبة المكتملة بناءً على تاريخ البدء المجدول وتواريخ الإكمال. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

يقوم بتحديث جميع الأعمال على أنها مكتملة حتى تاريخ محدد للقائمة المحددة من المهام.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| معامل | الوصف |
| --- | --- |
| completeThrough | التاريخ لتحديث العمل على أنه مكتمل حتى. |
| setZeroOrHundredPercentCompleteOnly | إذا تم تعيينه إلى true، يتم تحديث تلك المهام فقط إلى 100٪ مكتملة إذا كان تاريخ الانتهاء قبل تاريخ الإكمال المحدد. وإلا، يتم حساب قيمة النسبة المكتملة بناءً على تاريخ البدء المجدول وتواريخ الإكمال. |
| taskCollection | قائمة < Task > من المهام لتحديث العمل لها. |

