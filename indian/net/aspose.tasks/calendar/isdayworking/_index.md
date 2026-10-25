---
title: "Calendar.IsDayWorking"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्धारित करता है कि निर्दिष्ट दिन कैलेंडर के अनुसार कार्य दिवस है या नहीं"
type: docs
weight: 260
url: /hi/net/aspose.tasks/calendar/isdayworking/
---
## Calendar.IsDayWorking method

कैलेंडर के अनुसार निर्धारित करता है कि निर्दिष्ट दिन कार्य दिवस है या नहीं।

```csharp
public bool IsDayWorking(DateTime dt)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | DateTime | दिन कार्य दिवस है या नहीं जांचने के लिए तिथि। |

### रिटर्न वैल्यू

यदि दिन कार्य दिवस है तो सत्य।

## उदाहरण

दिखाता है कि कार्य घंटे कैसे गणना करें।

```csharp
var project = new Project(DataDir + "CalculateWorkHours.mpp");

// आईडी द्वारा टास्क तक पहुँचें
var task = project.RootTask.Children.GetById(1);

// कैलेंडर और उसके प्रारंभ और समाप्ति तिथियों तक पहुँचें
var taskCalendar = task.Get(Tsk.Calendar);
var startDate = task.Get(Tsk.Start);
var endDate = task.Get(Tsk.Finish);

// संसाधन और उनके कैलेंडर तक पहुँचें
var resource = project.Resources.GetByUid(1);
var resourceCalendar = resource.Get(Rsc.Calendar);

TimeSpan timeSpan;

// मिनट में अवधि प्राप्त करें
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

// घंटों में अवधि प्राप्त करें
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

// दिनों में अवधि प्राप्त करें
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

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


