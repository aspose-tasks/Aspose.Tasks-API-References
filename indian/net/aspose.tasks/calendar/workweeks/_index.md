---
title: "Calendar.WorkWeeks"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar प्रॉपर्टी। WorkWeekCollections ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी कार्य सप्ताहों का संग्रह।"
type: docs
weight: 130
url: /hi/net/aspose.tasks/calendar/workweeks/
---
## Calendar.WorkWeeks property

WorkWeekCollections ऑब्जेक्ट प्राप्त करता है। कैलेंडर से जुड़ी कार्य सप्ताहों का संग्रह।

```csharp
public WorkWeekCollection WorkWeeks { get; }
```

## उदाहरण

दिखाता है कि कार्य सप्ताह की जानकारी कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "WorkWithWorkWeekCollection.mpp");
var calendar = project.Calendars.GetByUid(1);

foreach (var workWeek in calendar.WorkWeeks)
{
    // कार्य सप्ताह का नाम, प्रारंभ और समाप्ति तिथियों को प्रदर्शित करें
    var name = workWeek.Name;
    var fromDate = workWeek.FromDate;
    var toDate = workWeek.ToDate;
    Console.WriteLine("Name: " + name);
    Console.WriteLine("From Date: " + fromDate);
    Console.WriteLine("To Date: " + toDate);

    // यह डेटा \"Details.\" बटन के बारे में है; आप विशेष सप्ताह के दिन के लिए विशेष कार्य समय सेट कर सकते हैं या इसे गैर-कार्यात्मक भी बना सकते हैं।
    foreach (var day in workWeek.WeekDays)
    {
        // आप कार्य समयों के माध्यम से आगे नेविगेट कर सकते हैं और इन्हें प्रदर्शित कर सकते हैं।
        foreach (var workingTime in day.WorkingTimes)
        {
            Console.WriteLine(workingTime.From);
            Console.WriteLine(workingTime.To);
        }
    }
}
```

### संबंधित देखें

* class [WorkWeekCollection](../../workweekcollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


