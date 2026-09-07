---
title: "Asn.LevelingDelay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Asn field. लेवलिंग के कारण हुई देरी"
type: docs
weight: 310
url: /hi/net/aspose.tasks/asn/levelingdelay/
---
## Asn.LevelingDelay field

लेवलिंग के कारण हुई देरी।

```csharp
public static readonly Key<Duration, AsnKey> LevelingDelay;
```

## उदाहरण

दिखाता है कि कैसे Asn.Delay और Asn.LevelingDelay प्रॉपर्टीज़ को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task 1");
task.Set(Tsk.Start, new DateTime(2000, 1, 3, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(8));

var resource = project.Resources.Add("Resource 1");

var assignment = project.ResourceAssignments.Add(task, resource);
assignment.Set(Asn.Delay, project.GetDuration(0, TimeUnitType.Day));

Console.WriteLine("Delay: " + assignment.Get(Asn.Delay));
Console.WriteLine("Leveling Delay: " + assignment.Get(Asn.LevelingDelay));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [AsnKey](../../asnkey/)
* class [Asn](../)
* namespace [Aspose.Tasks](../../asn/)
* assembly [Aspose.Tasks](../../../)


