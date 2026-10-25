---
title: "ResourceAssignment.GetTimephasedWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। निर्दिष्ट तिथि‑समय अंतराल के लिए टाइम‑फेज़्ड कार्य की मात्रा प्राप्त करता है"
type: docs
weight: 730
url: /hi/net/aspose.tasks/resourceassignment/gettimephasedwork/
---
## GetTimephasedWork(DateTime, DateTime, TimephasedDataType) {#gettimephasedwork_1}

निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है।

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end, 
    TimephasedDataType timephasedDataType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | तिथि‑समय अंतराल की शुरुआत। |
| समाप्ति | DateTime | तिथि‑समय अंतराल का अंत। |
| timephasedDataType | TimephasedDataType | उपयोग करने के लिए टाइम‑फेज़्ड डेटा का प्रकार। |

## उदाहरण

मनमाने तिथि‑समय अंतराल के लिए असाइनमेंट का कार्य कैसे गणना करें, यह दर्शाता है।

```csharp
var project = new Project(DataDir + "BaselineTD2010_3.mpp");

var assignment = project.ResourceAssignments.GetByUid(2);

// प्रत्येक घंटे के लिए असाइनमेंट का कार्य प्रिंट करें।
for (DateTime hour = assignment.Start; hour <= assignment.Finish; hour = hour.AddHours(1))
{
    var work = assignment.GetTimephasedWork(hour, hour.AddHours(1), TimephasedDataType.AssignmentWork);
    Console.WriteLine("{0} : {1:N2}", hour, work.TotalHours);
}
```

### संबंधित देखें

* enum [TimephasedDataType](../../timephaseddatatype/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)

---

## GetTimephasedWork(DateTime, DateTime) {#gettimephasedwork}

निर्दिष्ट तिथि-समय अंतराल के लिए टाइमफ़ेज़्ड कार्य की मात्रा प्राप्त करता है।

```csharp
public TimeSpan GetTimephasedWork(DateTime start, DateTime end)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | तिथि‑समय अंतराल की शुरुआत। |
| समाप्ति | DateTime | तिथि‑समय अंतराल का अंत। |

### संबंधित देखें

* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


