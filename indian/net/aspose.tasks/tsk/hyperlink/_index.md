---
title: "Tsk.Hyperlink"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य से जुड़े हाइपरलिंक के लिए शीर्षक या व्याख्यात्मक टेक्स्ट"
type: docs
weight: 490
url: /hi/net/aspose.tasks/tsk/hyperlink/
---
## Tsk.Hyperlink field

कार्य से संबंधित हाइपरलिंक के लिए शीर्षक या व्याख्यात्मक पाठ।

```csharp
public static readonly Key<string, TaskKey> Hyperlink;
```

## उदाहरण

दिखाता है कि Tsk.Hyperlink प्रॉपर्टीज़ को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Hyperlink, "Click here to visit our site");
task.Set(Tsk.HyperlinkAddress, "https://products.aspose.com");
task.Set(Tsk.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + task.Get(Tsk.Hyperlink));
Console.WriteLine("Hyperlink Address: " + task.Get(Tsk.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + task.Get(Tsk.HyperlinkSubAddress));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


