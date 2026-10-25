---
title: "RecurringInterval.MonthlyDayDayNumber"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringInterval प्रॉपर्टी। मासिक प्रोग्रेस लाइनों के दिन संख्या को प्राप्त करता है या सेट करता है।"
type: docs
weight: 60
url: /hi/net/aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/
---
## RecurringInterval.MonthlyDayDayNumber property

मासिक प्रगति रेखाओं के दिन संख्या को प्राप्त करता है या सेट करता है।

```csharp
public int MonthlyDayDayNumber { get; set; }
```

## उदाहरण

प्रगति रेखाओं के आवर्ती अंतराल के साथ कैसे काम करें, यह दिखाता है।

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

// प्रगति रेखा पढ़ने की अनुमति देता है।
var interval = view.ProgressLines.RecurringInterval;

Console.WriteLine("Interval: " + interval.Interval);
Console.WriteLine("Weekly Week Number: " + interval.WeeklyWeekNumber);
foreach (var day in interval.WeeklyDays)
{
    Console.WriteLine("Week day: " + day);
}

// आवर्ती अंतराल को पुनः परिभाषित करने की अनुमति देता है।
var newInterval = new RecurringInterval();

// एक मान सेट करता है जो दर्शाता है कि मासिक प्रगति रेखाएँ दिन के अनुसार दिखानी हैं या नहीं।
interval.MonthlyDay = true;
// मासिक प्रगति रेखाओं का दिनांक संख्या सेट करता है।
interval.MonthlyDayDayNumber = 1;
// मासिक प्रगति रेखाओं का माह संख्या सेट करता है।
interval.MonthlyDayMonthNumber = 1;
// एक मान सेट करता है जो दर्शाता है कि प्रगति रेखाएँ पहले या अंतिम पूर्वनिर्धारित दिन के अनुसार दिखानी हैं या नहीं।
interval.MonthlyFirstLast = true;
// मासिक प्रगति रेखाओं के पहले या अंतिम दिन प्रकार को सेट करता है।
interval.MonthlyFirstLastDay = RecurringInterval.DayType.Day;
// पहले या अंतिम पूर्वनिर्धारित दिन के अनुसार दिखायी जाने वाली प्रगति रेखाओं का माह संख्या सेट करता है।
interval.MonthlyFirstLastMonthNumber = 1;

view.ProgressLines.RecurringInterval = newInterval;

project.Save(OutDir + "WorkWithRecurringInterval_out.pdf", SaveFileFormat.Pdf);
```

### संबंधित देखें

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


