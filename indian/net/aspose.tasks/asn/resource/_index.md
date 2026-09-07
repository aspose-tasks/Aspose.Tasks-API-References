---
title: "Asn.Resource"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. कार्य को सौंपा गया संसाधन"
type: docs
weight: 470
url: /hi/net/aspose.tasks/asn/resource/
---
## Asn.Resource field

एक कार्य को सौंपा गया संसाधन।

```csharp
public static readonly Key<Resource, AsnKey> Resource;
```

## उदाहरण

दिखाता है कि कैसे Asn.Task और Asn.Resource प्रॉपर्टीज़ को पढ़ें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Assigned Task Name: " + assignment.Get(Asn.Task).Get(Tsk.Name));
Console.WriteLine("Assigned Resource Name: " + assignment.Get(Asn.Resource).Get(Rsc.Name));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* class [Resource](../../resource/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


