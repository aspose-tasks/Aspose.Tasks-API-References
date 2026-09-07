---
title: "Asn.FixedMaterial"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. निर्धारित करता है कि असाइन किए गए सामग्री संसाधन की खपत एक ही निश्चित मात्रा में होती है या नहीं"
type: docs
weight: 260
url: /hi/net/aspose.tasks/asn/fixedmaterial/
---
## Asn.FixedMaterial field

निर्धारित करता है कि क्या असाइन किए गए सामग्री संसाधन की खपत एक ही निश्चित मात्रा में होती है।

```csharp
public static readonly Key<bool, AsnKey> FixedMaterial;
```

## उदाहरण

दिखाता है कि Asn.FixedMaterial प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.FixedMaterial, true);

Console.WriteLine("Fixed Material: " + assignment.Get(Asn.FixedMaterial));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


