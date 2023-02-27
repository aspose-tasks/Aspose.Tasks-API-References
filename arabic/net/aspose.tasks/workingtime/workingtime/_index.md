---
title: WorkingTime.WorkingTime
second_title: Aspose.Tasks لمرجع .NET API
description: WorkingTime البناء. يقوم بتهيئة مثيل جديد لملفWorkingTime فئة مع فاصل زمني مع أوقات البدء والانتهاء المحددة .
type: docs
weight: 10
url: /ar/net/aspose.tasks/workingtime/workingtime/
---
## WorkingTime(DateTime, DateTime) {#constructor_1}

يقوم بتهيئة مثيل جديد لملف[`WorkingTime`](../) فئة مع فاصل زمني مع أوقات البدء والانتهاء المحددة .

```csharp
public WorkingTime(DateTime fromTime, DateTime toTime)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fromTime | DateTime | وقت بدء الفاصل الزمني |
| toTime | DateTime | وقت انتهاء الفاصل الزمني |

### أنظر أيضا

* class [WorkingTime](../)
* مساحة الاسم [Aspose.Tasks](../../workingtime/)
* المجسم [Aspose.Tasks](../../../)

---

## WorkingTime(TimeSpan, TimeSpan) {#constructor_2}

يقوم بتهيئة مثيل جديد لملف[`WorkingTime`](../) فئة مع عنصر فاصل زمني مع أوقات البدء والانتهاء المحددة.

```csharp
public WorkingTime(TimeSpan fromTime, TimeSpan toTime)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fromTime | TimeSpan | يتم تمثيل وقت بدء الفاصل الزمني بـTimeSpan هيكل. |
| toTime | TimeSpan | يتم تمثيل وقت انتهاء الفاصل الزمني بـTimeSpan هيكل. |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | عندما تكون toTime أقل من تساوي toTime الوسيطة أو عندما يكون الفاصل الزمني بين fromTime و toTime أكبر من 24 ساعة. |

### أمثلة

يمكن استخدام الحمل الزائد لـ WorkTime ctor لتهيئة بداية الفاصل الزمني ونهايته باستخدام TimeSpans:

```csharp
[C#]
var wt = new WorkingTime(new TimeSpan(9, 0, 0), new TimeSpan(18, 0, 0));
```

### أنظر أيضا

* class [WorkingTime](../)
* مساحة الاسم [Aspose.Tasks](../../workingtime/)
* المجسم [Aspose.Tasks](../../../)

---

## WorkingTime(int, int) {#constructor}

يقوم بتهيئة مثيل جديد لملف[`WorkingTime`](../) فئة مع عنصر فاصل زمني مع أوقات البدء والانتهاء المحددة.

```csharp
public WorkingTime(int fromHours, int toHours)
```

| معامل | يكتب | وصف |
| --- | --- | --- |
| fromHours | Int32 | يتم تمثيل وقت بدء الفاصل الزمني بعدد الساعات الكامل (0-24). |
| toHours | Int32 | يتم تمثيل وقت انتهاء الفاصل الزمني بعدد الساعات الكامل (0-24). |

### استثناءات

| استثناء | حالة |
| --- | --- |
| ArgumentException | عندما تكون toTime أقل من تساوي toTime الوسيطة أو عندما يكون الفاصل الزمني بين fromTime و toTime أكبر من 24 ساعة. |

### أمثلة

يمكن استخدام التحميل الزائد لـ WorkTime ctor لتهيئة بداية الفاصل الزمني ونهايته باستخدام ساعات كاملة:

```csharp
[C#]
var wt = new WorkingTime(9, 13);
```

### أنظر أيضا

* class [WorkingTime](../)
* مساحة الاسم [Aspose.Tasks](../../workingtime/)
* المجسم [Aspose.Tasks](../../../)


