---
title: "Enum CalculationMode"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.CalculationMode enum. प्रोजेक्ट कैलकुलेशन मोड को निर्दिष्ट करता है"
type: docs
weight: 210
url: /hi/net/aspose.tasks/calculationmode/
---
## CalculationMode enumeration

परियोजना गणना मोड को निर्दिष्ट करता है।

```csharp
public enum CalculationMode
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| None | `0` | None. इस मोड में प्रोजेक्ट की तिथियों और लागतों को पुनः गणना नहीं की जाती है। |
| Automatic | `1` | Automatic mode. इस मोड का उपयोग करने पर प्रोजेक्ट की तिथियों और लागतों को पुनः गणना किया जाता है। |
| Manual | `2` | Manual mode. इस मोड में केवल आवश्यक फ़ील्ड्स को पुनः गणना किया जाता है, जैसे कि ऑब्जेक्ट्स के UIDs और IDs। |

## उदाहरण

ऑटो कैलकुलेशन मोड का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.Automatic
};

// प्रोजेक्ट की प्रारंभ तिथि सेट करें और नई टास्क जोड़ें
project.Set(Prj.StartDate, new DateTime(2015, 4, 15));
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");

// टास्क को लिंक करें
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);

// तिथियों की पुनः गणना की पुष्टि करें
Console.WriteLine("Task1 Start + 1 Equals Task2 Start : {0} ", task1.Get(Tsk.Start).AddDays(1).Equals(task2.Get(Tsk.Start)));
Console.WriteLine("Task1 Finish + 1 Equals Task2 Finish : {0} ", task1.Get(Tsk.Finish).AddDays(1).Equals(task2.Get(Tsk.Finish)));
Console.WriteLine("RootTask Finish Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.RootTask.Get(Tsk.Finish)));
Console.WriteLine("Project Finish Date Equals Task2 Finish : {0} ", task2.Get(Tsk.Finish).Equals(project.Get(Prj.FinishDate)));
```

None कैलकुलेशन मोड का उपयोग कैसे करें, यह दिखाता है।

```csharp
var project = new Project
{
    CalculationMode = CalculationMode.None
};

// एक नई टास्क जोड़ें
var task = project.RootTask.Children.Add("Task");

// ध्यान दें कि यहाँ तक कि IDs भी गणना नहीं किए गए थे            
Console.WriteLine("Task.Id Equals 0 : {0} ", task.Get(Tsk.Id).Equals(0));
Console.WriteLine("Task.OutlineLevel Equals 0 : {0} ", task.Get(Tsk.OutlineLevel).Equals(0));
Console.WriteLine("Task Start Equals DateTime.MinValue : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
Console.WriteLine("Task Duration Equals 0 mins : {0} ", task.Get(Tsk.Duration).ToString().Equals("0 mins"));

// ड्यूरेशन प्रॉपर्टी सेट करें
task.Set(Tsk.Duration, project.GetDuration(2, TimeUnitType.Day));
Console.WriteLine("Task Duration Equals 2 days : {0} ", task.Get(Tsk.Duration).ToString().Equals("2 days"));
Console.WriteLine("Task Start Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Start).Equals(DateTime.MinValue));
Console.WriteLine("Task Finish Equals DateTime.MinValue  : {0} ", task.Get(Tsk.Finish).Equals(DateTime.MinValue));
```

Manual कैलकुलेशन मोड का उपयोग कैसे करें, यह दिखाता है।

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


