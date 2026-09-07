---
title: "एनम TaskType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskType एनम। कार्य के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 2470
url: /hi/net/aspose.tasks/tasktype/
---
## TaskType enumeration

टास्क के प्रकार को निर्दिष्ट करता है।

```csharp
public enum TaskType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| Undefined | `-1` | अपरिभाषित मान का अर्थ है कि फ़ील्ड मूल फ़ाइल में परिभाषित नहीं था |
| FixedUnits | `0` | स्थिर इकाइयाँ |
| FixedDuration | `1` | स्थिर अवधि |
| FixedWork | `2` | स्थिर कार्य |

## टिप्पणियाँ

XML में निर्यात करते समय अपरिभाषित मानों को परिणामी XML से हटा दिया जाएगा।

## उदाहरण

दिखाता है कि प्रोजेक्ट की डिफ़ॉल्ट प्रॉपर्टीज़ कैसे पढ़ें।

```csharp
var project = new Project(DataDir + "DefaultProperties.mpp");

// डिफ़ॉल्ट प्रॉपर्टीज़ सेट करें
project.Set(Prj.ScheduleFromStart, true);
project.Set(Prj.StartDate, DateTime.Now);
project.Set(Prj.DefaultStartTime, project.Get(Prj.StartDate));
project.Set(Prj.DefaultTaskType, TaskType.FixedDuration);
project.Set(Prj.DefaultStandardRate, 15);
project.Set(Prj.DefaultOvertimeRate, 12);
project.Set(Prj.DefaultTaskEVMethod, EarnedValueMethodType.PercentComplete);
project.Set(Prj.DefaultFixedCostAccrual, CostAccrualType.Prorated);

// डिफ़ॉल्ट प्रॉपर्टीज़ प्रदर्शित करें
Console.WriteLine("New Task Default Start: " + project.Get(Prj.DefaultStartTime).ToShortDateString());
Console.WriteLine("New Task Default Type: " + project.Get(Prj.DefaultTaskType));
Console.WriteLine("Resource Default Standard Rate: " + project.Get(Prj.DefaultStandardRate));
Console.WriteLine("Resource Default Overtime Rate: " + project.Get(Prj.DefaultOvertimeRate));
Console.WriteLine("Default Task EV Method: " + project.Get(Prj.DefaultTaskEVMethod));
Console.WriteLine("Default Cost Accrual: " + project.Get(Prj.DefaultFixedCostAccrual));
```

### संबंधित देखें

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


