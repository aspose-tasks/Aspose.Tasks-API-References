---
title: "Rsc.Workgroup"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc फ़ील्ड। वह कार्यसमूह का प्रकार जिससे कोई संसाधन संबंधित है"
type: docs
weight: 700
url: /hi/net/aspose.tasks/rsc/workgroup/
---
## Rsc.Workgroup field

संसाधन जिस कार्यसमूह से संबंधित है, उसका प्रकार।

```csharp
public static readonly Key<WorkGroupType, RscKey> Workgroup;
```

## उदाहरण

दिखाता है कि Rsc.Workgroup प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.Workgroup, WorkGroupType.Email);

Console.WriteLine("Workgroup: " + resource.Get(Rsc.Workgroup));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [WorkGroupType](../../workgrouptype/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


