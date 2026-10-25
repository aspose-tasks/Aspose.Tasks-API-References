---
title: "Asn.Task"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। वह कार्य जिससे एक संसाधन सौंपा गया है।"
type: docs
weight: 550
url: /hi/net/aspose.tasks/asn/task/
---
## Asn.Task field

वह कार्य जिससे एक संसाधन सौंपा गया है।

```csharp
public static readonly Key<Task, AsnKey> Task;
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
* class [Task](../../task/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


