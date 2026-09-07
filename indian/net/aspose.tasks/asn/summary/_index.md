---
title: "Asn.Summary"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. निर्धारित करता है कि कार्य सारांश कार्य है या नहीं"
type: docs
weight: 530
url: /hi/net/aspose.tasks/asn/summary/
---
## Asn.Summary field

निर्धारित करता है कि कार्य एक सारांश कार्य है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> Summary;
```

## उदाहरण

दिखाता है कि Asn.Summary प्रॉपर्टी कैसे पढ़ें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Summary, true);

Console.WriteLine("Summary: " + assignment.Get(Asn.Summary));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


