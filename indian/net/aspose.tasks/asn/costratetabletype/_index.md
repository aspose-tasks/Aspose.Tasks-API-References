---
title: "Asn.CostRateTableType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। इस असाइनमेंट के लिए उपयोग की गई लागत दर तालिका"
type: docs
weight: 190
url: /hi/net/aspose.tasks/asn/costratetabletype/
---
## Asn.CostRateTableType field

इस असाइनमेंट के लिए उपयोग की गई लागत दर तालिका।

```csharp
public static readonly Key<RateType, AsnKey> CostRateTableType;
```

## उदाहरण

दिखाता है कि Asn.CostRateTableType प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.CostRateTableType, RateType.B);

Console.WriteLine("Cost Rate Table Type: " + assignment.Get(Asn.CostRateTableType));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [RateType](../../ratetype/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


