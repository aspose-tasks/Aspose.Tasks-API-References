---
title: "Asn.LinkedFields"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. निर्धारित करता है कि प्रोजेक्ट किसी अन्य OLE ऑब्जेक्ट से जुड़ा है या नहीं"
type: docs
weight: 320
url: /hi/net/aspose.tasks/asn/linkedfields/
---
## Asn.LinkedFields field

निर्धारित करता है कि प्रोजेक्ट किसी अन्य OLE ऑब्जेक्ट से जुड़ा है या नहीं।

```csharp
public static readonly Key<bool, AsnKey> LinkedFields;
```

## उदाहरण

Asn.LinkedFields प्रॉपर्टी को कैसे पढ़ें दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);

Console.WriteLine("Linked Fields: " + assignment.Get(Asn.LinkedFields));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


