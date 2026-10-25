---
title: "Asn.VAC"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. बेसलाइन लागत और कुल लागत के बीच अंतर"
type: docs
weight: 590
url: /hi/net/aspose.tasks/asn/vac/
---
## Asn.VAC field

बेसलाइन लागत और कुल लागत के बीच अंतर।

```csharp
public static readonly Key<double, AsnKey> VAC;
```

## उदाहरण

दिखाता है कि कैसे Asn.VAC प्रॉपर्टी को पढ़ें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.VAC, 10);

Console.WriteLine("VAC: " + assignment.Get(Asn.VAC));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


