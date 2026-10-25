---
title: "Prj.DaysPerMonth"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। महीने में दिनों की संख्या"
type: docs
weight: 220
url: /hi/net/aspose.tasks/prj/dayspermonth/
---
## Prj.DaysPerMonth field

प्रति माह दिनों की संख्या।

```csharp
public static readonly Key<int, PrjKey> DaysPerMonth;
```

## उदाहरण

दिखाता है कि प्रोजेक्ट के सप्ताह के दिन की प्रॉपर्टीज़ को कैसे पढ़ें/लिखें।

```csharp
var project = new Project(DataDir + "WriteWeekdayProperties.mpp");

// सप्ताह के दिनों की प्रॉपर्टीज़ सेट करें
project.Set(Prj.WeekStartDay, DayType.Monday);
project.Set(Prj.DaysPerMonth, 24);
project.Set(Prj.MinutesPerDay, 540);
project.Set(Prj.MinutesPerWeek, 3240);

// सप्ताह के दिनों की प्रॉपर्टीज़ प्रदर्शित करें
Console.WriteLine("Week Start Date: " + project.Get(Prj.WeekStartDay));
Console.WriteLine("Days Per Month: " + project.Get(Prj.DaysPerMonth));
Console.WriteLine("Minutes Per Day: " + project.Get(Prj.MinutesPerDay));
Console.WriteLine("Minutes Per Week: " + project.Get(Prj.MinutesPerWeek));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


