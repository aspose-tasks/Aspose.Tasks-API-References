---
title: "Rsc.ActualOvertimeWorkProtected"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Rsc field. वास्तविक ओवरटाइम कार्य की सुरक्षा करने वाला कार्य की मात्रा"
type: docs
weight: 60
url: /hi/net/aspose.tasks/rsc/actualovertimeworkprotected/
---
## Rsc.ActualOvertimeWorkProtected field

वह कार्य मात्रा जिसके माध्यम से वास्तविक ओवरटाइम कार्य संरक्षित रहता है।

```csharp
public static readonly Key<Duration, RscKey> ActualOvertimeWorkProtected;
```

## उदाहरण

दिखाता है कि Rsc.ActualOvertimeWorkProtected प्रॉपर्टी को कैसे पढ़ें/लिखें.

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var resource = project.Resources.Add("Resource");

resource.Set(Rsc.ActualOvertimeWorkProtected, project.GetWork(1));

Console.WriteLine("Actual Overtime Work Protected: " + resource.Get(Rsc.ActualOvertimeWorkProtected));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [RscKey](../../rsckey/)
* class [Rsc](../)
* namespace [Aspose.Tasks](../../rsc/)
* assembly [Aspose.Tasks](../../../)


