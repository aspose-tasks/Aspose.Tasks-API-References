---
title: "Calendar.IsDayWorking"
second_title: "مرجع API لـ Aspose.Tasks لـ .NET"
description: "طريقة Calendar. تحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم"
type: docs
weight: 260
url: /ar/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

يحدد ما إذا كان اليوم المحدد يوم عمل وفقًا للتقويم.

```csharp
public bool IsDayWorking(DateTime dt)
```

| معامل | النوع | الوصف |
| --- | --- | --- |
| dt | DateTime | التاريخ للتحقق مما إذا كان اليوم عملًا. |

### قيمة الإرجاع

صحيح إذا كان اليوم يوم عمل.

## الأمثلة

يعرض كيفية حساب ساعات العمل.

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// الوصول إلى المهمة بواسطة المعرف
var task = project.RootTask.Children.GetById(1);

// الوصول إلى Calendar وتواريخ بدايته ونهايته
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// الوصول إلى المورد وتقويمه
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// احصل على المدة بالدقائق
double durationInMins = 0;
var tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInMins += timeSpan.TotalMinutes;
    }

    tempDate = tempDate.AddDays(1);
}

tempDate = startDate;

// احصل على المدة بالساعات
double durationInHours = 0;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        durationInHours += timeSpan.TotalHours;
    }

    tempDate = tempDate.AddDays(1);
}

// احصل على المدة بالأيام
double durationInDays = 0;
tempDate = startDate;
while (tempDate < endDate)
{
    if (taskCalendar.IsDayWorking(tempDate) && resourceCalendar.IsDayWorking(tempDate))
    {
        timeSpan = taskCalendar.GetWorkingHours(tempDate);
        if (timeSpan.TotalHours > 0)
        {
            durationInDays += timeSpan.TotalDays * (24 / timeSpan.TotalHours);
        }
    }

    tempDate = tempDate.AddDays(1);
}

Console.WriteLine("Duration in Minutes = " + durationInMins);
Console.WriteLine("Duration in Hours = " + durationInHours);
Console.WriteLine("Duration in Days = " + durationInDays);
```

### انظر أيضًا

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


