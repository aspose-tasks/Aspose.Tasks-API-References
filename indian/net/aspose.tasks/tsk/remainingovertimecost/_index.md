---
title: "Tsk.RemainingOvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के लिए शेष निर्धारित ओवरटाइम खर्च"
type: docs
weight: 970
url: /hi/net/aspose.tasks/tsk/remainingovertimecost/
---
## Tsk.RemainingOvertimeCost field

कार्य के लिए शेष निर्धारित ओवरटाइम खर्च।

```csharp
public static readonly Key<decimal, TaskKey> RemainingOvertimeCost;
```

## उदाहरण

दिखाता है कि कैसे Tsk.RemainingOvertimeCost प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.RemainingOvertimeCost, 2m);

Console.WriteLine("Remaining Overtime Cost: " + task.Get(Tsk.RemainingOvertimeCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


