---
title: "Asn.RegularWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. असाइनमेंट के लिए निर्धारित गैर‑ओवरटाइम कार्य की मात्रा"
type: docs
weight: 420
url: /hi/net/aspose.tasks/asn/regularwork/
---
## Asn.RegularWork field

एक असाइनमेंट के लिए निर्धारित गैर-ओवरटाइम कार्य की मात्रा।

```csharp
public static readonly Key<Duration, AsnKey> RegularWork;
```

## उदाहरण

दिखाता है कि कैसे Asn.RegularWork प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.RegularWork, project.GetWork(1));

Console.WriteLine("Regular Work: " + assignment.Get(Asn.RegularWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


