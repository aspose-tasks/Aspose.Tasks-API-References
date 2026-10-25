---
title: "ResourceAssignment.Get"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment विधि. इस कंटेनर में गुण को मैप किया गया मान लौटाता है"
type: docs
weight: 700
url: /hi/net/aspose.tasks/resourceassignment/get/
---
## ResourceAssignment.Get&lt;T&gt; method

इस कंटेनर में प्रॉपर्टी जिस मान पर मैप की गई है, वह मान लौटाता है।

```csharp
public T Get<T>(Key<T, AsnKey> key)
```

| पैरामीटर | विवरण |
| --- | --- |
| T | मैप किए गए मान का प्रकार। |
| key | निर्दिष्ट प्रॉपर्टी कुंजी। प्रॉपर्टी कुंजी प्राप्त करने के लिए [`Asn`](../../asn/)। |

### रिटर्न वैल्यू

वह मान जिससे यह प्रॉपर्टी इस कंटेनर में मैप की गई है।

## उदाहरण

एक असाइनमेंट बनाने और सामान्य असाइनमेंट गुणों को प्राप्त/सेट करने का तरीका दर्शाता है।

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var task = project.RootTask.Children.Add("Task");
task.Set(Tsk.Start, new DateTime(2020, 4, 2, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(1));
task.Set(Tsk.Finish, new DateTime(2020, 4, 2, 17, 0, 0));
var resource = project.Resources.Add("Resource");
var resourceAssignment = project.ResourceAssignments.Add(task, resource);
resourceAssignment.Set(Asn.Start, new DateTime(2020, 4, 2, 8, 0, 0));
resourceAssignment.Set(Asn.Work, project.GetWork(1));
resourceAssignment.Set(Asn.Finish, new DateTime(2020, 4, 2, 17, 0, 0));

Console.WriteLine(resourceAssignment.Get(Asn.Start));
Console.WriteLine(resourceAssignment.Get(Asn.Work));
Console.WriteLine(resourceAssignment.Get(Asn.Finish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


