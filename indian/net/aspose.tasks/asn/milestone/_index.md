---
title: "Asn.Milestone"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। निर्धारित करता है कि असाइनमेंट एक माइलस्टोन है या नहीं।"
type: docs
weight: 330
url: /hi/net/aspose.tasks/asn/milestone/
---
## Asn.Milestone field

निर्धारित करता है कि असाइनमेंट एक माइलस्टोन है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> Milestone;
```

## उदाहरण

दिखाता है कि कैसे Asn.Milestone प्रॉपर्टी को पढ़ें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Milestone: " + assignment.Get(Asn.Milestone));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


