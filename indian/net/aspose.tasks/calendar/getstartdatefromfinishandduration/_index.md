---
title: "Calendar.GetStartDateFromFinishAndDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है"
type: docs
weight: 200
url: /hi/net/aspose.tasks/calendar/getstartdatefromfinishandduration/
---
## GetStartDateFromFinishAndDuration(DateTime, Duration) {#getstartdatefromfinishandduration}

निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है।

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, Duration duration)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| समाप्ति | DateTime | निर्दिष्ट समाप्ति तिथि। |
| अवधि | अवधि | निर्दिष्ट अवधि। |

### रिटर्न वैल्यू

गणना की गई प्रारंभ तिथि।

## उदाहरण

दिखाता है कि समाप्ति तिथि और अवधि के द्वारा प्रारंभ तिथि कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// समाप्ति तिथि और अवधि द्वारा प्रारंभ तिथि प्राप्त करें
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), project.GetDuration(16, TimeUnitType.Hour));

// 8 अप्रैल 2020 9:00 AM प्रिंट किया जाएगा
Console.WriteLine(startDate);
```

### संबंधित देखें

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetStartDateFromFinishAndDuration(DateTime, TimeSpan) {#getstartdatefromfinishandduration_1}

निर्दिष्ट समाप्ति तिथि और अवधि के आधार पर प्रारंभ तिथि लौटाता है।

```csharp
public DateTime GetStartDateFromFinishAndDuration(DateTime finish, TimeSpan duration)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| समाप्ति | DateTime | निर्दिष्ट समाप्ति तिथि। |
| अवधि | TimeSpan | निर्दिष्ट अवधि। |

### रिटर्न वैल्यू

गणना की गई प्रारंभ तिथि।

## उदाहरण

दिखाता है कि समाप्ति तिथि और अवधि (समय अंतराल के रूप में) द्वारा प्रारंभ तिथि कैसे प्राप्त करें।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// समाप्ति तिथि और अवधि द्वारा प्रारंभ तिथि प्राप्त करें
var startDate = calendar.GetStartDateFromFinishAndDuration(new DateTime(2020, 4, 10, 9, 0, 0), TimeSpan.FromHours(16));

// 8 अप्रैल 2020 9:00 AM प्रिंट किया जाएगा
Console.WriteLine(startDate);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


