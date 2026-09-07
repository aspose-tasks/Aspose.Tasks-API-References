---
title: "Prj.DefaultStandardRate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। नए संसाधनों के लिए डिफ़ॉल्ट मानक दर"
type: docs
weight: 260
url: /hi/net/aspose.tasks/prj/defaultstandardrate/
---
## Prj.DefaultStandardRate field

नई संसाधनों के लिए डिफ़ॉल्ट मानक दर।

```csharp
public static readonly Key<double, PrjKey> DefaultStandardRate;
```

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

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


