---
title: "WeekDay.WeekDay"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "منشئ WeekDay. يهيئ مثيلًا جديدًا من فئة WeekDay بالنوع اليوم المحدد"
type: docs
weight: 10
url: /ar/net/aspose.tasks/weekday/weekday/
---
## WeekDay(DayType) {#constructor_1}

يهيئ مثيلًا جديدًا من الفئة [`WeekDay`](../) بالنوع اليوم المحدد.

```csharp
public WeekDay(DayType dayType)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dayType | DayType | نوع اليوم المحدد. |

## الأمثلة

يظهر كيفية إنشاء تقويم جديد عن طريق تعريف أيام الأسبوع.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// تحقق من تواريخ البداية والنهاية ليوم الاستثناء
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير

// يضبط وقت العمل. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// هناك طريقة لتحويل <see cref="DayOfWeek" /> إلى <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// لنطبع جميع أوقات العمل
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### انظر أيضًا

* enum [DayType](../../daytype/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, IEnumerable&lt;WorkingTime&gt;) {#constructor_3}

يهيئ مثيلًا جديدًا من الفئة [`WeekDay`](../) بالنوع اليوم المحدد وقائمة فترات وقت العمل.

```csharp
public WeekDay(DayType dayType, IEnumerable<WorkingTime> workingTimes)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dayType | DayType | نوع اليوم المحدد. |
| workingTimes | IEnumerable`1 | قائمة فترات وقت العمل. |

## الأمثلة

يظهر كيفية إنشاء تقويم جديد عن طريق تعريف أيام الأسبوع.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// تحقق من تواريخ البداية والنهاية ليوم الاستثناء
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير

// يضبط وقت العمل. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// هناك طريقة لتحويل <see cref="DayOfWeek" /> إلى <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// لنطبع جميع أوقات العمل
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### انظر أيضًا

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay(DayType, params WorkingTime[]) {#constructor_2}

يهيئ مثيلًا جديدًا من الفئة [`WeekDay`](../) بالنوع اليوم المحدد وفترات وقت العمل.

```csharp
public WeekDay(DayType dayType, params WorkingTime[] workingTimes)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dayType | DayType | نوع اليوم المحدد. |
| workingTimes | WorkingTime[] | مصفوفة فترات وقت العمل. |

### انظر أيضًا

* enum [DayType](../../daytype/)
* class [WorkingTime](../../workingtime/)
* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)

---

## WeekDay() {#constructor}

يهيئ مثيلًا جديدًا من الفئة [`WeekDay`](../).

```csharp
public WeekDay()
```

## الأمثلة

يظهر كيفية إنشاء تقويم جديد عن طريق تعريف أيام الأسبوع.

```csharp
var project = new Project();

// تعريف تقويم
var calendar = project.Calendars.Add("Calendar1");

// إضافة أيام العمل من الاثنين إلى الخميس مع الأوقات الافتراضية
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Monday));
calendar.WeekDays.Add(new WeekDay(DayType.Tuesday, new WorkingTime(9, 11), new WorkingTime(12, 18)));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Wednesday));
calendar.WeekDays.Add(WeekDay.CreateDefaultWorkingDay(DayType.Thursday));

var exceptionDay = WeekDay.CreateDefaultWorkingDay(DayType.Exception);
exceptionDay.FromDate = new DateTime(2020, 4, 27, 0, 0, 0);
exceptionDay.ToDate = new DateTime(2020, 4, 30, 0, 0, 0);
exceptionDay.DayWorking = false;
calendar.WeekDays.Add(exceptionDay);

// تحقق من تواريخ البداية والنهاية ليوم الاستثناء
Console.WriteLine("The from date is: " + exceptionDay.FromDate);
Console.WriteLine("The to date is: " + exceptionDay.ToDate);
Console.WriteLine();

calendar.WeekDays.Add(new WeekDay(DayType.Saturday));
calendar.WeekDays.Add(new WeekDay(DayType.Sunday));

// تعيين الجمعة كيوم عمل قصير

// يضبط وقت العمل. 
var workingTimes = new List<WorkingTime> { new WorkingTime(9, 12), new WorkingTime(13, 16) };

// هناك طريقة لتحويل <see cref="DayOfWeek" /> إلى <see cref="Aspose.Tasks.DayType" />.
var dayType = WeekDay.CastToDayType(DayOfWeek.Friday);

var weekDay = new WeekDay(dayType, workingTimes);
weekDay.DayWorking = true;
Console.WriteLine("The day type is: " + weekDay.DayType);
Console.WriteLine("The from date is: " + weekDay.FromDate);
Console.WriteLine("The to date is: " + weekDay.ToDate);

calendar.WeekDays.Add(weekDay);

// لنطبع جميع أوقات العمل
foreach (var day in calendar.WeekDays)
{
    Console.WriteLine("Day Type: " + day.DayType); 
    Console.WriteLine("Is working day: " + day.DayWorking); 
    Console.WriteLine("Working Time (Hours): " + day.GetWorkingTime().TotalHours);
    Console.WriteLine();
}
```

### انظر أيضًا

* class [WeekDay](../)
* namespace [Aspose.Tasks](../../weekday/)
* assembly [Aspose.Tasks](../../../)


