---
title: "Asn.HasFixedRateUnits"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn फ़ील्ड। निर्धारित करता है कि यूनिट्स में फिक्स्ड रेट है या नहीं।"
type: docs
weight: 270
url: /hi/net/aspose.tasks/asn/hasfixedrateunits/
---
## Asn.HasFixedRateUnits field

निर्धारित करता है कि इकाइयों की दर निश्चित है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> HasFixedRateUnits;
```

## उदाहरण

दिखाता है कि कैसे Asn.HasFixedRateUnits प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.HasFixedRateUnits, true);

Console.WriteLine("Has Fixed Rate Units: " + assignment.Get(Asn.HasFixedRateUnits));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


