---
title: "Enum TaskStartDateType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskStartDateType enum. टास्क की प्रारंभ तिथि के प्रकार को निर्दिष्ट करता है"
type: docs
weight: 2450
url: /hi/net/aspose.tasks/taskstartdatetype/
---
## TaskStartDateType enumeration

टास्क की प्रारंभ तिथि के प्रकार को निर्दिष्ट करता है।

```csharp
public enum TaskStartDateType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | फ़ील्ड का मान मूल प्रोजेक्ट फ़ाइल में परिभाषित नहीं था। |
| ProjectStartDate | `0` | प्रोजेक्ट प्रारंभ तिथि |
| CurrentDate | `1` | वर्तमान तिथि |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि टास्क की डिफ़ॉल्ट प्रारंभ तिथि को 'CurrentDate' के रूप में कैसे सेट करें।

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);
project.Save(OutDir + "SetAttributesForNewTasks_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


