---
title: "Aspose::Tasks::TaskCollection::Add طريقة"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks لـ C++"
description: "يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس مستوى المخطط للمهمة الأخيرة."
type: docs
weight: 10
url: /ar/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس مستوى المخطط للمهمة الأخيرة.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

يدرج مهمة جديدة قبل مهمة ذات المعرف المحدد وعلى نفس مستوى المخطط.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| معامل | الوصف |
| --- | --- |
| معلمات | المعلمات المحددة لإنشاء مهمة متكررة. |

---

## Add (3 of 5) {#add_3}

أضف المهمة المحددة إلى نسخة فئة TaskCollection. إذا كان ParentProject.CalculationMode يساوي None يجب على المستخدم استدعاء Project.Recalculate() بعد استخدام هذه الطريقة (ستعيد جدولة جميع مهام المشروع (تواريخ البدء/الانتهاء، وتحدد تواريخ مبكرة/متأخرة) وتحسب الحقول التابعة مثل الفجوات، والعمل، وتكاليف الحقول، والمعرفات ومستويات المخطط). إذا كان ParentProject.CalculationMode يساوي Manual فإن الطريقة ستحسب فقط معرف المهمة، ومستوى المخطط، وأرقام المخطط تلقائيًا. إذا كان ParentProject.CalculationMode يساوي Automatic فإن الطريقة تعيد جدولة جميع مهام المشروع تلقائيًا (تواريخ البدء/الانتهاء، وتحدد تواريخ مبكرة/متأخرة، وتحسب الفجوات، والعمل، وتكاليف الحقول، وتعيد حساب المعرفات ومستويات المخطط).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| معامل | الوصف |
| --- | --- |
| العنصر | المهمة المحددة التي يجب إضافتها إلى مجموعة المهام هذه. |

---

## Add (4 of 5) {#add_4}

يضيف مهمة جديدة إلى مجموعة مهام الأطفال.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| معامل | الوصف |
| --- | --- |
| taskName | اسم المهمة المحدد. |

---

## Add (5 of 5) {#add_5}

يضيف مهمة متكررة جديدة إلى مجموعة مهام الأطفال.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| معامل | الوصف |
| --- | --- |
| taskName | اسم المهمة المحدد. |
| beforeTaskId | معرف المهمة المحدد الذي سيُدرج قبله مهمة جديدة. |

