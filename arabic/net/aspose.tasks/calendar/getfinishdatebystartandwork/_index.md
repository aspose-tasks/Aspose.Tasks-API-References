---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تحسب التاريخ الذي سينقضي فيه مقدار الوقت العمل المحدد وفقًا للتقويم."
type: docs
weight: 160
url: /ar/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء. |
| العمل | المدة | مدة العمل. |

### قيمة الإرجاع

تاريخ الانتهاء.

## الأمثلة

يظهر كيفية حساب تاريخ الانتهاء بناءً على تاريخ البدء والعمل باستخدام نسخة من Calendar.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// احسب تاريخ الانتهاء باستخدام تقويم قياسي
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### انظر أيضًا

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

يحسب التاريخ الذي سينقضي فيه مقدار وقت العمل المحدد وفقًا للتقويم.

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| بداية | DateTime | تاريخ البدء. |
| العمل | TimeSpan | مدة العمل. |

### قيمة الإرجاع

تاريخ الانتهاء.

## الأمثلة

يظهر كيفية حساب تاريخ الانتهاء بناءً على تاريخ البدء والعمل (كفترة زمنية) باستخدام نسخة من Calendar.

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// احسب تاريخ الانتهاء باستخدام تقويم قياسي
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


