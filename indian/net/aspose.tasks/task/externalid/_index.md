---
title: "Task.ExternalId"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Task property. ExternalId का मान प्राप्त करता है या सेट करता है"
type: docs
weight: 410
url: /hi/net/aspose.tasks/task/externalid/
---
## Task.ExternalId property

प्राप्त करता है या सेट करता है ExternalId का मान।

```csharp
public int ExternalId { get; set; }
```

## उदाहरण

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

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


