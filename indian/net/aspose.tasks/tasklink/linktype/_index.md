---
title: "TaskLink.LinkType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskLink प्रॉपर्टी। लिंक के प्रकार को प्राप्त करता है या सेट करता है"
type: docs
weight: 60
url: /hi/net/aspose.tasks/tasklink/linktype/
---
## TaskLink.LinkType property

एक लिंक के प्रकार को प्राप्त करता है या सेट करता है।

```csharp
public TaskLinkType LinkType { get; set; }
```

## उदाहरण

दिखाता है कि कार्य लिंक के लिंक प्रकार को कैसे प्राप्त/सेट करें।

```csharp
var project = new Project();

// नए कार्य जोड़ें।
var pred = project.RootTask.Children.Add("Task 1");
var succ = project.RootTask.Children.Add("Task 2");

// कार्य को लिंक करें जहाँ लिंक प्रकार स्टार्ट टू स्टार्ट सेट हो।
var newLink = project.TaskLinks.Add(pred, succ);
newLink.LinkType = TaskLinkType.StartToStart;

foreach (var link in project.TaskLinks)
{
    Console.WriteLine("Task Link Type: " + link.LinkType.ToString());
}
```

### संबंधित देखें

* enum [TaskLinkType](../../tasklinktype/)
* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


