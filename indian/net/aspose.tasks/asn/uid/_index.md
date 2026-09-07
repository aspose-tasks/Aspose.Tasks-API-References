---
title: "Asn.Uid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। एक असाइनमेंट का अद्वितीय पहचानकर्ता।"
type: docs
weight: 560
url: /hi/net/aspose.tasks/asn/uid/
---
## Asn.Uid field

एक असाइनमेंट का अद्वितीय पहचानकर्ता।

```csharp
public static readonly Key<int, AsnKey> Uid;
```

## उदाहरण

दिखाता है कि **Asn.Uid** प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");
resource.Set(Rsc.Type, ResourceType.Work);

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Uid, 30);

Console.WriteLine("UID: " + assignment.Get(Asn.Uid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


