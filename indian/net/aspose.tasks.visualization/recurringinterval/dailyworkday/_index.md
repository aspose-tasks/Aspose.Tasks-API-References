---
title: "RecurringInterval.DailyWorkday"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "RecurringInterval प्रॉपर्टी। एक मान प्राप्त करता है या सेट करता है जो यह दर्शाता है कि क्या कोई दिन दैनिक प्रोग्रेस लाइनों के लिए कार्यदिवस है।"
type: docs
weight: 30
url: /hi/net/aspose.tasks.visualization/recurringinterval/dailyworkday/
---
## RecurringInterval.DailyWorkday property

यह दर्शाने वाला मान प्राप्त करता है या सेट करता है कि दैनिक प्रोग्रेस लाइनों के लिए कोई दिन कार्य दिवस है या नहीं।

```csharp
public bool DailyWorkday { get; set; }
```

## उदाहरण

प्रोग्रेस लाइनों के दैनिक आवर्ती अंतराल को जोड़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "Project2007.mpp");
project.Set(Prj.StatusDate, project.Get(Prj.StartDate));

var view = (GanttChartView)project.Views.ToList()[1];

view.ProgressLines.RecurringInterval = new RecurringInterval();
// दैनिक पैटर्न दिन संख्या सेट करें
view.ProgressLines.RecurringInterval.DailyDayNumber = 2;
// एक मान सेट करें जो यह दर्शाता है कि क्या कोई दिन दैनिक प्रोग्रेस लाइनों के लिए कार्यदिवस है।
view.ProgressLines.RecurringInterval.DailyWorkday = true;
```

### संबंधित देखें

* class [RecurringInterval](../)
* namespace [Aspose.Tasks.Visualization](../../recurringinterval/)
* assembly [Aspose.Tasks](../../../)


