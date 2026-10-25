---
title: "क्लास RecurringInterval"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.Visualization.RecurringInterval क्लास। गैंट चार्ट दृश्य की प्रोग्रेस लाइनों में उपयोग किए जाने वाले आवर्ती अंतराल का प्रतिनिधित्व करता है।"
type: docs
weight: 3310
url: /hi/net/aspose.tasks.visualization/recurringinterval/
---
## RecurringInterval class

गैंट चार्ट दृश्य में प्रोग्रेस लाइनों में उपयोग किए जाने वाले आवर्ती अंतराल को दर्शाता है।

```csharp
public class RecurringInterval
```

## कन्स्ट्रक्टर्स

| नाम | विवरण |
| --- | --- |
| [RecurringInterval](recurringinterval/)() | डिफ़ॉल्ट कन्स्ट्रक्टर। |

## गुण

| नाम | विवरण |
| --- | --- |
| [DailyDayNumber](../../aspose.tasks.visualization/recurringinterval/dailydaynumber/) { get; set; } | दैनिक दिन संख्या प्राप्त करता है या सेट करता है। |
| [DailyWorkday](../../aspose.tasks.visualization/recurringinterval/dailyworkday/) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि दैनिक प्रोग्रेस लाइनों के लिए कोई दिन कार्य दिवस है या नहीं। |
| [Interval](../../aspose.tasks.visualization/recurringinterval/interval/) { get; set; } | आवर्ती अंतराल प्राप्त करता है या सेट करता है। यह [`Interval`](./interval/) प्रकार का कोई भी मान हो सकता है। |
| [MonthlyDay](../../aspose.tasks.visualization/recurringinterval/monthlyday/) { get; set; } | यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि मासिक प्रोग्रेस लाइनों को दिन के अनुसार दिखाया जाए या नहीं। |
| [MonthlyDayDayNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaydaynumber/) { get; set; } | मासिक प्रगति रेखाओं के दिन संख्या को प्राप्त करता है या सेट करता है। |
| [MonthlyDayMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlydaymonthnumber/) { get; set; } | मासिक प्रगति रेखाओं के महीने संख्या को प्राप्त करता है या सेट करता है। |
| [MonthlyFirstLast](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlast/) { get; set; } | पहले या अंतिम पूर्वनिर्धारित दिन के अनुसार प्रगति रेखाओं को दिखाने का संकेत देने वाले मान को प्राप्त करता है या सेट करता है। |
| [MonthlyFirstLastDay](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastday/) { get; set; } | मासिक प्रगति रेखाओं के पहले या अंतिम दिन प्रकार को प्राप्त करता है या सेट करता है। |
| [MonthlyFirstLastMonthNumber](../../aspose.tasks.visualization/recurringinterval/monthlyfirstlastmonthnumber/) { get; set; } | पहले या अंतिम पूर्वनिर्धारित दिन के अनुसार दिखाए जाने वाली प्रगति रेखाओं के महीने संख्या को प्राप्त करता है या सेट करता है। |
| [WeeklyDays](../../aspose.tasks.visualization/recurringinterval/weeklydays/) { get; } | साप्ताहिक प्रगति रेखाओं के लिए दिनों की सूची प्राप्त करता है। |
| [WeeklyWeekNumber](../../aspose.tasks.visualization/recurringinterval/weeklyweeknumber/) { get; set; } | साप्ताहिक प्रगति रेखाओं के सप्ताह संख्या को प्राप्त करता है या सेट करता है। |

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

* namespace [Aspose.Tasks.Visualization](../../aspose.tasks.visualization/)
* assembly [Aspose.Tasks](../../)


