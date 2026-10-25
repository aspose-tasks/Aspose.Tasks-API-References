---
title: "Calendar.GetWorkingHours"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar मेथड। निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की WorkUnit, प्रारंभ, समाप्ति और अवधि लौटाता है।"
type: docs
weight: 220
url: /hi/net/aspose.tasks/calendar/getworkinghours/
---
## GetWorkingHours(DateTime, DateTime) {#getworkinghours}

वर्कयूनिट लौटाता है - निर्दिष्ट तिथि-समय अंतराल के लिए कार्य घंटे की शुरुआत, समाप्ति और अवधि।

```csharp
public WorkUnit GetWorkingHours(DateTime start, DateTime finish)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | अंतराल की प्रारंभ तिथि। |
| समाप्ति | DateTime | अंतराल की समाप्ति तिथि। |

### रिटर्न वैल्यू

[`WorkUnit`](../../workunit/) क्लास का उदाहरण जिसमें कार्य घंटे की प्रारंभ, समाप्ति और अवधि शामिल है।

## उदाहरण

विशिष्ट तिथियों के लिए कार्य घंटे प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// विशिष्ट तिथि के लिए कार्य घंटे प्राप्त करें
var workUnit = calendar.GetWorkingHours(new DateTime(2020, 4, 8, 8, 0, 0), new DateTime(2020, 4, 9, 17, 0, 0));

// 16 घंटे प्रदर्शित किए जाएंगे
Console.WriteLine(workUnit.WorkingHours);
```

### संबंधित देखें

* class [WorkUnit](../../workunit/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetWorkingHours(DateTime) {#getworkinghours_1}

निर्दिष्ट तिथि पर कार्य घंटे की मात्रा लौटाता है।

```csharp
public TimeSpan GetWorkingHours(DateTime dt)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| dt | DateTime | कार्य घंटे प्राप्त करने के लिए तिथि। |

### रिटर्न वैल्यू

निर्दिष्ट तिथि पर कार्य घंटे।

## उदाहरण

एक विशिष्ट तिथि के लिए कार्य घंटे प्राप्त करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project1.mpp");

var calendar = project.Calendars.GetByUid(1);

// विशिष्ट तिथि के लिए कार्य घंटे प्राप्त करें
var workingHours = calendar.GetWorkingHours(new DateTime(2020, 4, 10));

// 8 घंटे प्रिंट किए जाएंगे
Console.WriteLine(workingHours.Hours);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


