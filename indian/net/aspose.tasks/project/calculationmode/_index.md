---
title: "Project.CalculationMode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project प्रॉपर्टी। प्रोजेक्ट की गणना मोड प्राप्त करता है या सेट करता है। यह CalculationMode एन्यूमरेशन के मानों में से एक हो सकता है"
type: docs
weight: 110
url: /hi/net/aspose.tasks/project/calculationmode/
---
## Project.CalculationMode property

प्रोजेक्ट की गणना मोड प्राप्त करता है या सेट करता है। यह `CalculationMode` एन्यूमरेशन के मानों में से एक हो सकता है।

```csharp
public CalculationMode CalculationMode { get; set; }
```

## उदाहरण

प्रोजेक्ट गणना मोड का उपयोग करने का तरीका दिखाता है।

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Manual
};

// प्रोजेक्ट की प्रारंभ तिथि सेट करें और नई टास्क जोड़ें
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// आवश्यक प्रॉपर्टीज़ मैनुअल मोड में सेट की गई हैं
Console.WriteLine("Task1.Id Equals 1 : {0} ", task1.Get(Tsk.Id).Equals(1));
Console.WriteLine("Task1 OutlineLevel Equals 1 : {0} ", task1.Get(Tsk.OutlineLevel).Equals(1));
Console.WriteLine("Task1 Start Equals 15/04/2015 08:00 AM : {0} ", task1.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task1 Finish Equals 15/04/2015 05:00 PM : {0} ", task1.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task1 Duration Equals 1 day : {0} ", task1.Get(Tsk.Duration).ToString().Equals("1 day"));
Console.WriteLine("Task2 Start Equals 15/04/2015 08:00 AM : {0} ", task2.Get(Tsk.Start).Equals(new DateTime(2015, 4, 15, 8, 0, 0)));
Console.WriteLine("Task2 Finish Equals 15/04/2015 05:00 PM : {0} ", task2.Get(Tsk.Finish).Equals(new DateTime(2015, 4, 15, 17, 0, 0)));
Console.WriteLine("Task2 Duration Equals 1 day : {0} ", task2.Get(Tsk.Duration).ToString().Equals("1 day"));

// जब हम दो टास्क को लिंक करते हैं तो उनके तिथियों को मैनुअल मोड में पुनः गणना नहीं की जाती है
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// टास्क 2 की शुरुआत में कोई परिवर्तन नहीं हुआ है
Console.WriteLine("Task1 Start Equals Task2 Start : {0} ", task1.Get(Tsk.Start).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).Equals(task2.Get(Tsk.Finish)));
```

### संबंधित देखें

* enum [CalculationMode](../../calculationmode/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


