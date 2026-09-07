---
title: "Prj.NewTaskStartDate"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Prj फ़ील्ड। नए कार्यों के लिए डिफ़ॉल्ट प्रारंभ तिथि प्रकार"
type: docs
weight: 580
url: /hi/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

नई कार्यों के लिए डिफ़ॉल्ट प्रारंभ तिथि प्रकार।

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## उदाहरण

नए कार्यों के लिए गुण सेट करने का तरीका दिखाता है।

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


