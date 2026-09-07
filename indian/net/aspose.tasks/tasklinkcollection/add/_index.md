---
title: "TaskLinkCollection.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLinkCollection मेथड। FinishStart TaskLink का एक इंस्टेंस लौटाता है जिसे TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है"
type: docs
weight: 40
url: /hi/net/aspose.tasks/tasklinkcollection/add/
---
## Add(Task, Task) {#add}

एक Finish-Start [`TaskLink`](../../tasklink/) का उदाहरण लौटाता है जो TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

```csharp
public TaskLink Add(Task pred, Task succ)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | कार्य | पूर्ववर्ती कार्य। |
| succ | कार्य | उत्तराधिकारी कार्य। |

### रिटर्न वैल्यू

एक टास्क लिंक उदाहरण जो इस ऑब्जेक्ट में जोड़ा गया है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | यदि किसी इनपुट टास्क का मान null है तो ArgumentNullException फेंका जाएगा। |

## उदाहरण

टास्क लिंक कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// टास्क प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// टास्क को लिंक करें
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// टास्कों के बीच लिंक प्रिंट करें
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// इंडेक्स एक्सेस द्वारा लिंक संपादित करें
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// सभी टास्क लिंक हटाएँ
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### संबंधित देखें

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType) {#add_1}

एक [`TaskLink`](../../tasklink/) का उदाहरण लौटाता है जो TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | कार्य | पूर्ववर्ती कार्य। |
| succ | कार्य | उत्तराधिकारी कार्य। |
| linkType | TaskLinkType | लिंक प्रकार [`TaskLinkType`](../../tasklinktype/) |

### रिटर्न वैल्यू

एक टास्क लिंक उदाहरण जो इस ऑब्जेक्ट में जोड़ा गया है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | यदि किसी इनपुट टास्क का मान null है तो ArgumentNullException फेंका जाएगा। |

## उदाहरण

टास्क लिंक कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// टास्क प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// टास्क को लिंक करें
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// टास्कों के बीच लिंक प्रिंट करें
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// इंडेक्स एक्सेस द्वारा लिंक संपादित करें
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// सभी टास्क लिंक हटाएँ
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### संबंधित देखें

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(Task, Task, TaskLinkType, Duration) {#add_2}

एक [`TaskLink`](../../tasklink/) का उदाहरण लौटाता है जो TaskLinkCollection ऑब्जेक्ट में जोड़ा गया है।

```csharp
public TaskLink Add(Task pred, Task succ, TaskLinkType linkType, Duration lag)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| pred | कार्य | पूर्ववर्ती कार्य। |
| succ | कार्य | उत्तराधिकारी कार्य। |
| linkType | TaskLinkType | लिंक प्रकार [`TaskLinkType`](../../tasklinktype/) |
| lag | Duration | लिंक लैग [`Duration`](../../duration/). |

### रिटर्न वैल्यू

एक टास्क लिंक जो इस ऑब्जेक्ट में जोड़ा गया है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | यदि किसी इनपुट टास्क का मान null है तो ArgumentNullException फेंका जाएगा। |

## उदाहरण

टास्क लिंक कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "SampleProject.mpp");

// टास्क प्राप्त करें
var task1 = project.RootTask.Children.GetById(1);
var task2 = project.RootTask.Children.GetById(2);
var task3 = project.RootTask.Children.GetById(3);
var task4 = project.RootTask.Children.GetById(4);
var task5 = project.RootTask.Children.GetById(5);

// टास्क को लिंक करें
project.TaskLinks.Add(task1, task2);
project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart, project.GetDuration(1, TimeUnitType.Day));
project.TaskLinks.Add(task2, task5, TaskLinkType.FinishToStart, project.GetDuration(2, TimeUnitType.Day));

// टास्कों के बीच लिंक प्रिंट करें
Console.WriteLine("Print task links of " + project.TaskLinks.ParentProject.Get(Prj.Name) + " project.");
Console.WriteLine("Task links count: " + project.TaskLinks.Count);
foreach (var link in project.TaskLinks)
{
    Console.WriteLine("From ID = " + link.PredTask.Get(Tsk.Id) + " => To ID = " + link.SuccTask.Get(Tsk.Id));
    Console.WriteLine();
}

// इंडेक्स एक्सेस द्वारा लिंक संपादित करें
project.TaskLinks[0].LagFormat = TimeUnitType.Hour;

// सभी टास्क लिंक हटाएँ
List<TaskLink> taskLinks = project.TaskLinks.ToList();
foreach (var link in taskLinks)
{
    project.TaskLinks.Remove(link);
}
```

### संबंधित देखें

* class [TaskLink](../../tasklink/)
* class [Task](../../task/)
* enum [TaskLinkType](../../tasklinktype/)
* struct [Duration](../../duration/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(TaskLink) {#add_3}

यह ICollection की Add मेथड की स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकती है।

```csharp
public void Add(TaskLink item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | TaskLink | जोड़ने के लिए आइटम। |

### संबंधित देखें

* class [TaskLink](../../tasklink/)
* class [TaskLinkCollection](../)
* namespace [Aspose.Tasks](../../tasklinkcollection/)
* assembly [Aspose.Tasks](../../../)


