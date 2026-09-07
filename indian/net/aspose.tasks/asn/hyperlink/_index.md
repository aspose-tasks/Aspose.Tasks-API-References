---
title: "Asn.Hyperlink"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. असाइनमेंट से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ"
type: docs
weight: 280
url: /hi/net/aspose.tasks/asn/hyperlink/
---
## Asn.Hyperlink field

असाइनमेंट से जुड़े हाइपरलिंक का शीर्षक या व्याख्यात्मक पाठ।

```csharp
public static readonly Key<string, AsnKey> Hyperlink;
```

## उदाहरण

Shows how to read/write hyperlink properties. हाइपरलिंक प्रॉपर्टीज़ को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Hyperlink, "Click to visit our site");
assignment.Set(Asn.HyperlinkAddress, "https://products.aspose.com");
assignment.Set(Asn.HyperlinkSubAddress, "/total/net");

Console.WriteLine("Hyperlink: " + assignment.Get(Asn.Hyperlink));
Console.WriteLine("Hyperlink Address: " + assignment.Get(Asn.HyperlinkAddress));
Console.WriteLine("Hyperlink Sub Address: " + assignment.Get(Asn.HyperlinkSubAddress));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


