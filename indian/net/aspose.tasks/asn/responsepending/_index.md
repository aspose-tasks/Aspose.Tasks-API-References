---
title: "Asn.ResponsePending"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. निर्धारित करता है कि TeamAssign संदेश के लिए प्रतिक्रिया प्राप्त हुई है या नहीं"
type: docs
weight: 480
url: /hi/net/aspose.tasks/asn/responsepending/
---
## Asn.ResponsePending field

निर्धारित करता है कि TeamAssign संदेश के लिए प्रतिक्रिया प्राप्त हुई है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> ResponsePending;
```

## उदाहरण

Shows how to read/write Asn.ResponsePending property. दिखाता है कि Asn.ResponsePending प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.ResponsePending, true);

Console.WriteLine("Response Pending: " + assignment.Get(Asn.ResponsePending));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


