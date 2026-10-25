---
title: "Project.GetDuration"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Project. تحصل على كائن Duration مع العدد المحدد من الوحدات وتنسيق المدة الافتراضي المحدد في إعدادات المشروع DurationFormat"
type: docs
weight: 1100
url: /ar/net/aspose.tasks/project/getduration/
---
## GetDuration(double) {#getduration}

تحصل على كائن [`Duration`](../../duration/) مع العدد المحدد من الوحدات وتنسيق المدة الافتراضي المحدد في إعدادات المشروع [`DurationFormat`](../../prj/durationformat/).

```csharp
public Duration GetDuration(double val)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Double | عدد الوحدات المحدد. |

### قيمة الإرجاع

كائن Duration.

## ملاحظات

يجب استخدام هذه الطريقة بحذر لأنها تُعيد مددًا مختلفة اعتمادًا على إعداد Project.DurationFormat. على سبيل المثال، GetWork(1.0) سيعيد 1 ساعة عندما يكون Project.DurationFormat هو TimeUnitType.Hour أو 1 يوم إذا كان Project.DurationFormat هو TimeUnitType.Day.

## الأمثلة

يظهر كيفية إنشاء نسخة &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; باستخدام تنسيق مدة المشروع الافتراضي عبر طرق نسيج المشروع.

```csharp
var project = new Project();

// احصل على مدة بتنسيق المشروع الافتراضي.
var duration = project.GetDuration(1);

Console.WriteLine("Default project duration time unit type: " + project.Get(Prj.DurationFormat));
Console.WriteLine("Created duration time unit type: " + duration.TimeUnit);
```

### انظر أيضًا

* struct [Duration](../../duration/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(double, TimeUnitType) {#getduration_1}

تحصل على كائن [`Duration`](../../duration/) مع العدد المحدد من وحدات [`TimeUnitType`](../../timeunittype/).

```csharp
public Duration GetDuration(double val, TimeUnitType timeUnit)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| القيمة | Double | عدد الوحدات المحدد. |
| timeUnit | TimeUnitType | قيمة TimeUnitType المحددة. |

### قيمة الإرجاع

كائن Duration.

## الأمثلة

يظهر كيفية إنشاء نسخة &lt;see cref=\"Aspose.Tasks.Duration\" /&gt; باستخدام طرق نسيج المشروع.

```csharp
var project = new Project();

// احصل على مدة بتنسيق المشروع الافتراضي.
var duration = project.GetDuration(1, TimeUnitType.Minute);

Console.WriteLine("Created duration: " + duration);
```

### انظر أيضًا

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## GetDuration(TimeSpan, TimeUnitType) {#getduration_2}

تحصل على كائن [`Duration`](../../duration/) مع قيمة TimeSpan المحددة وقيمة [`TimeUnitType`](../../timeunittype/) المحددة.

```csharp
public Duration GetDuration(TimeSpan timeSpan, TimeUnitType timeUnit)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| timeSpan | TimeSpan | قيمة TimeSpan المحددة. |
| timeUnit | TimeUnitType | قيمة TimeUnitType المحددة. |

### قيمة الإرجاع

كائن Duration.

### انظر أيضًا

* struct [Duration](../../duration/)
* enum [TimeUnitType](../../timeunittype/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


