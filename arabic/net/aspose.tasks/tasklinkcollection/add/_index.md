---
title: TaskLinkCollection.Add
second_title: Aspose.Tasks لمرجع .NET API
description: TaskLinkCollection طريقة. إرجاع مثيل لـ FinishStartTaskLink التي تمت إضافتها إلى كائن TaskLinkCollection.
type: docs
weight: 40
url: /ar/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

إرجاع مثيل لـ Finish-Start[`TaskLink`](../../tasklink/) التي تمت إضافتها إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pred | Task | المهمة السابقة. |
| succ | Task | مهمة الوريث. |

### قيمة الإرجاع

نسخة ارتباط مهمة تمت إضافتها إلى هذا الكائن.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي فارغًاArgumentNullException سوف يتم إلقاؤها. |

### أنظر أيضا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* مساحة الاسم [Aspose.Tasks](../../tasklinkcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

إرجاع مثيل لـ[`TaskLink`](../../tasklink/) التي تمت إضافتها إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pred | Task | المهمة السابقة. |
| succ | Task | مهمة الوريث. |
| linkType | TaskLinkType | نوع الارتباط[`TaskLinkType`](../../tasklinktype/) |

### قيمة الإرجاع

نسخة ارتباط مهمة تمت إضافتها إلى هذا الكائن.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي فارغًاArgumentNullException سوف يتم إلقاؤها. |

### أنظر أيضا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* مساحة الاسم [Aspose.Tasks](../../tasklinkcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

إرجاع مثيل لـ[`TaskLink`](../../tasklink/) التي تمت إضافتها إلى كائن TaskLinkCollection.

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| pred | Task | المهمة السابقة. |
| succ | Task | مهمة الوريث. |
| linkType | TaskLinkType | نوع الارتباط[`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | ارتباط تأخر[`Duration`](../../duration/). |

### قيمة الإرجاع

ارتباط مهمة تمت إضافته إلى هذا الكائن.

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentNullException | إذا كان أي من مهام الإدخال يساوي فارغًاArgumentNullException سوف يتم إلقاؤها. |

### أنظر أيضا

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* مساحة الاسم [Aspose.Tasks](../../tasklinkcollection/)
* المجسم [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

هذا هو تنفيذ كعب الروتين لطريقة Add الخاصة بـ ICollection ، والتي ترمي فقط NotSupportedException

```csharp
public void Add(TaskLink item)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| item | TaskLink | العنصر المراد إضافته. |

### أنظر أيضا

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* مساحة الاسم [Aspose.Tasks](../../tasklinkcollection/)
* المجسم [Aspose.Tasks](../../../)


