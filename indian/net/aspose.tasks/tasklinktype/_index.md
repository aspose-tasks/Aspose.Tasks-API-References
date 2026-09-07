---
title: "एनम TaskLinkType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskLinkType एनम। कार्य निर्भरता के प्रकार को निर्दिष्ट करता है।"
type: docs
weight: 2440
url: /hi/net/aspose.tasks/tasklinktype/
---
## TaskLinkType enumeration

टास्क निर्भरता के प्रकार को निर्दिष्ट करता है।

```csharp
public enum TaskLinkType
```

### मान

| नाम | मान | विवरण |
| --- | --- | --- |
| FinishToFinish | `0` | फ़िनिश-फ़िनिश संबंध |
| FinishToStart | `1` | फ़िनिश-स्टार्ट संबंध |
| StartToFinish | `2` | स्टार्ट-फ़िनिश संबंध |
| StartToStart | `3` | स्टार्ट-स्टार्ट संबंध |

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

* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


