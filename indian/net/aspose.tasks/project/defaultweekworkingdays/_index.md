---
title: "Project.DefaultWeekWorkingDays"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। WeekDayCollection क्लास का इंस्टेंस प्राप्त करता है जो प्रोजेक्ट के डिफ़ॉल्ट साप्ताहिक कार्य दिवसों और कार्य समयों का संग्रह दर्शाता है।"
type: docs
weight: 370
url: /hi/net/aspose.tasks/project/defaultweekworkingdays/
---
## Project.DefaultWeekWorkingDays property

[`WeekDayCollection`](../../weekdaycollection/) क्लास का इंस्टेंस प्राप्त करता है जो प्रोजेक्ट के डिफ़ॉल्ट साप्ताहिक कार्य दिवसों और कार्य समयों का संग्रह दर्शाता है।

```csharp
public WeekDayCollection DefaultWeekWorkingDays { get; }
```

### रिटर्न वैल्यू

यह [`WeekDayCollection`](../../weekdaycollection/) क्लास का इंस्टेंस है जिसमें [`WeekDay`](../../weekday/) ऑब्जेक्ट्स की सूची शामिल है।

## टिप्पणियाँ

डेटा केवल mpp फ़ाइलों में मौजूद है (xml में नहीं)।

## उदाहरण

दिखाता है कि डिफ़ॉल्ट साप्ताहिक कार्य दिवस कैसे प्राप्त किया जाए।

```csharp
var project = new Project(DataDir + "Project2003.mpp");
foreach (var weekDay in project.DefaultWeekWorkingDays)
{
    Console.WriteLine("From: " + weekDay.FromDate);
    Console.WriteLine("From: " + weekDay.ToDate);
    Console.WriteLine("Day type: " + weekDay.DayType);
    Console.WriteLine("Is day working: " + weekDay.DayWorking);
}
```

### संबंधित देखें

* class [WeekDayCollection](../../weekdaycollection/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


