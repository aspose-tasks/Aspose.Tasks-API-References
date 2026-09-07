---
title: "Tsk.IsExternalTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि कार्य बाहरी है या नहीं"
type: docs
weight: 600
url: /hi/net/aspose.tasks/tsk/isexternaltask/
---
## Tsk.IsExternalTask field

निर्धारित करता है कि कार्य बाहरी है या नहीं।

```csharp
public static readonly Key<bool, TaskKey> IsExternalTask;
```

## उदाहरण

दिखाता है कि कैसे Tsk.IsExternalTask प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsExternalTask, true);

Console.WriteLine("Is External Task: " + task.Get(Tsk.IsExternalTask));
```

दिखाता है कि कैसे क्रॉस प्रोजेक्ट कार्य लिंक बनाया जाए - किसी अन्य (बाहरी) प्रोजेक्ट में कार्य का लिंक।

```csharp
Project project = new Project();
var summary = project.RootTask.Children.Add("Summary Task");

// किसी अन्य प्रोजेक्ट से कार्य के लिंक को बनाने के लिए हमें बनाना चाहिए
// वर्तमान प्रोजेक्ट में उसका डुप्लिकेट (या "external") कार्य।

Task t2 = summary.Children.Add("External Task");
t2.Set(Tsk.ExternalTaskProject, "ExternalProject.mpp"); // here we set path to external project's MPP file.
t2.Set(Tsk.ExternalId, 1); // Set External task's Id.
t2.Set(Tsk.ExternalUid, 2); // External task's Unique Id should be set.
t2.Set(Tsk.IsExternalTask, true);
t2.Set(Tsk.IsManual, new NullableBool(false));
t2.Set(Tsk.IsSummary, false);

Task t = summary.Children.Add("Task");
TaskLink link = project.TaskLinks.Add(t2, t);
link.IsCrossProject = true;
link.LinkType = TaskLinkType.FinishToStart;
link.CrossProjectName = "ExternalProject.mpp\\\\1"; // <- here external task's Id is used.
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


