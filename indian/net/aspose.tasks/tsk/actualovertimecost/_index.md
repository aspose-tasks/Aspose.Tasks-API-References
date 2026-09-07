---
title: "Tsk.ActualOvertimeCost"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। असाइन किए गए संसाधनों द्वारा कार्यों पर पहले से किए गए ओवरटाइम कार्य के लिए हुए खर्च"
type: docs
weight: 50
url: /hi/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

असाइन किए गए रिसोर्स द्वारा टास्क पर पहले से किए गए ओवरटाइम कार्य के लिए हुए खर्च।

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## उदाहरण

दिखाता है कि Tsk.ActualOvertimeCost प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


