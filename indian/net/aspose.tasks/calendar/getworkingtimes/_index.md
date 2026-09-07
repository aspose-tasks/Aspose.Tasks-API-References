---
title: "Calendar.GetWorkingTimes"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्दिष्ट तिथि के लिए कार्य समय की WorkingTimeCollection लौटाता है"
type: docs
weight: 240
url: /hi/net/aspose.tasks/calendar/getworkingtimes/
---
## Calendar.GetWorkingTimes method

निर्दिष्ट तिथि के लिए कार्य समयों की [`WorkingTimeCollection`](../../workingtimecollection/) लौटाता है।

```csharp
public WorkingTimeCollection GetWorkingTimes(DateTime dt)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | DateTime | कार्य समय प्राप्त करने के लिए तिथि। |

### रिटर्न वैल्यू

[`WorkingTime`](../../workingtime/) के उदाहरणों का संग्रह।

## उदाहरण

विशिष्ट तिथि के लिए कार्य समय प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// विशिष्ट तिथि के लिए कार्य समय प्राप्त करें
var workingTimes = calendar.GetWorkingTimes(new DateTime(2020, 4, 8, 8, 0, 0));

// 16 घंटे प्रदर्शित किए जाएंगे
foreach (var workingTime in workingTimes)
{
    Console.WriteLine("From: " + workingTime.From);
    Console.WriteLine("To: " + workingTime.To);
}
```

### संबंधित देखें

* class [WorkingTimeCollection](../../workingtimecollection/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


