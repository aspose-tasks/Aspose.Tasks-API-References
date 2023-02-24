---
title: TaskCollection.Add
second_title: Aspose.Tasks لمرجع .NET API
description: TaskCollection طريقة. أضف المهمة المحددة إلى مثيل ملفTaskCollectionclass. إذا كان ParentProject.CalculationMode هو لا شيء يجب على المستخدم استدعاء Project.Recalculate  بعد استخدام هذه الطريقة ستعيد جدولة جميع مهام المشروع تواريخ البدء / الانتهاء  وتعيين التواريخ المبكرة / المتأخرة وحساب الحقول التابعة مثل فترات العمل  والعمل وحقول التكلفة والمعرفات ومستويات المخطط التفصيلي . إذا كان ParentProject.CalculationMode هو يدوي  فستقوم الطريقة بحساب معرف المهمة فقط  ومستوى المخطط التفصيلي وأرقام المخطط التفصيلي تلقائيًا. التواريخ  وتعيين التواريخ المبكرة / المتأخرة  وتحسب فترات الركود  وحقول العمل والتكلفة  وإعادة حساب المعرفات ومستويات المخطط التفصيلي.
type: docs
weight: 50
url: /ar/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

أضف المهمة المحددة إلى مثيل ملف[`TaskCollection`](../)class. إذا كان ParentProject.CalculationMode هو لا شيء يجب على المستخدم استدعاء Project.Recalculate () بعد استخدام هذه الطريقة (ستعيد جدولة جميع مهام المشروع (تواريخ البدء / الانتهاء ، وتعيين التواريخ المبكرة / المتأخرة) وحساب الحقول التابعة مثل فترات العمل ، والعمل وحقول التكلفة والمعرفات ومستويات المخطط التفصيلي) . إذا كان ParentProject.CalculationMode هو يدوي ، فستقوم الطريقة بحساب معرف المهمة فقط ، ومستوى المخطط التفصيلي وأرقام المخطط التفصيلي تلقائيًا. التواريخ ، وتعيين التواريخ المبكرة / المتأخرة ، وتحسب فترات الركود ، وحقول العمل والتكلفة ، وإعادة حساب المعرفات ومستويات المخطط التفصيلي).

```csharp
public void Add(Task item)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| item | Task | المهمة المحددة التي يجب إضافتها إلى مجموعة المهام هذه. |

### أنظر أيضا

* class [Task](../../task/)
* class [TaskCollection](../)
* مساحة الاسم [Aspose.Tasks](../../taskcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add() {#add}

يضيف مهمة جديدة إلى مجموعة مهام المشروع على نفس مستوى المخطط التفصيلي للمهمة الأخيرة.

```csharp
public Task Add()
```

### قيمة الإرجاع

يُرجع المثيل المضاف حديثًا لـ[`Task`](../../task/) فصل.

### أنظر أيضا

* class [Task](../../task/)
* class [TaskCollection](../)
* مساحة الاسم [Aspose.Tasks](../../taskcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

يضيف مهمة جديدة لمجموعة مهام الأطفال.

```csharp
public Task Add(string taskName)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| taskName | String | اسم المهمة المحدد. |

### قيمة الإرجاع

يُرجع المثيل المضاف حديثًا لـ[`Task`](../../task/) فصل.

### أنظر أيضا

* class [Task](../../task/)
* class [TaskCollection](../)
* مساحة الاسم [Aspose.Tasks](../../taskcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

يضيف مهمة متكررة جديدة لمجموعة المهام الفرعية.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| taskName | String | اسم المهمة المحدد. |
| beforeTaskId | Int32 | المعرف المحدد للمهمة التي سيتم إدراج مهمة جديدة قبلها. |

### قيمة الإرجاع

تقوم بإرجاع مهمة تم إدراجها قبل مهمة بالمعرف المحدد.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentOutOfRangeException | يتم طرح ArgumentOutOfRangeException إذا كان المعرف المحدد ليس معرف مهمة صالحًا. |

### أنظر أيضا

* class [Task](../../task/)
* class [TaskCollection](../)
* مساحة الاسم [Aspose.Tasks](../../taskcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

لإدراج مهمة جديدة قبل مهمة بالمعرف المحدد وعلى نفس مستوى المخطط التفصيلي.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| parameters | RecurringTaskParameters | المعلمات المعلمات المحددة لإنشاء مهمة متكررة. |

### قيمة الإرجاع

يُرجع المثيل المضاف حديثًا لـ[`Task`](../../task/) فصل.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | يتم إلقاؤها إذا كانت المعلمات المحددة خالية. |
| ArgumentException | يتم إلقاؤها إذا كانت المعلمات المحددة غير صالحة. |

### أنظر أيضا

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* مساحة الاسم [Aspose.Tasks](../../taskcollection/)
* المجسم [Aspose.Tasks](../../../)


