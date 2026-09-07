---
title: "Calendar.GetFinishDateByStartAndWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Calendar विधि। कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने की तिथि की गणना करती है"
type: docs
weight: 160
url: /hi/net/aspose.tasks/calendar/getfinishdatebystartandwork/
---
## GetFinishDateByStartAndWork(DateTime, Duration) {#getfinishdatebystartandwork}

कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है।

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, Duration work)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | प्रारंभ तिथि। |
| कार्य | अवधि | कार्य अवधि। |

### रिटर्न वैल्यू

समाप्ति तिथि।

## उदाहरण

दिखाता है कि कैलेंडर इंस्टेंस का उपयोग करके शुरू तिथि और कार्य के आधार पर समाप्ति तिथि कैसे गणना करें।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// मानक कैलेंडर का उपयोग करके समाप्ति तिथि की गणना करें
var finish = calendar.GetFinishDateByStartAndWork(start, work);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### संबंधित देखें

* struct [Duration](../../duration/)
* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)

---

## GetFinishDateByStartAndWork(DateTime, TimeSpan) {#getfinishdatebystartandwork_1}

कैलेंडर के अनुसार निर्दिष्ट कार्य समय की मात्रा समाप्त होने पर तिथि की गणना करता है।

```csharp
public DateTime GetFinishDateByStartAndWork(DateTime start, TimeSpan work)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | प्रारंभ तिथि। |
| कार्य | TimeSpan | कार्य अवधि। |

### रिटर्न वैल्यू

समाप्ति तिथि।

## उदाहरण

दिखाता है कि कैलेंडर इंस्टेंस का उपयोग करके शुरू तिथि और कार्य (समय अंतराल के रूप में) के आधार पर समाप्ति तिथि कैसे गणना करें।

```csharp
var project = new Project(DataDir + "Blank2010.mpp");

var calendar = project.Calendars.GetByName("Standard");

var start = new DateTime(2017, 10, 26, 8, 0, 0);
var work = project.GetWork(7);

// मानक कैलेंडर का उपयोग करके समाप्ति तिथि की गणना करें
var finish = calendar.GetFinishDateByStartAndWork(start, work.TimeSpan);

Console.WriteLine("Task start date: " + start);
Console.WriteLine("Task work: " + work);
Console.WriteLine("Task finish date: " + finish);
```

### संबंधित देखें

* class [Calendar](../)
* namespace [Aspose.Tasks](../../calendar/)
* assembly [Aspose.Tasks](../../../)


