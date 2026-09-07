---
title: "Tsk.LevelingDelay"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. वह समय जब कोई कार्य संसाधन लेवलिंग के कारण अपनी प्रारंभिक तिथि से विलंबित किया जाता है"
type: docs
weight: 770
url: /hi/net/aspose.tasks/tsk/levelingdelay/
---
## Tsk.LevelingDelay field

संसाधन लेवलिंग के कारण कार्य को उसके प्रारंभिक प्रारंभ तिथि से विलंबित किया जाने वाला समय।

```csharp
public static readonly Key<Duration, TaskKey> LevelingDelay;
```

## उदाहरण

दिखाता है कि कैसे Tsk.LevelingDelay प्रॉपर्टी को पढ़ा/लिखा जाए।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingDelay, project.GetDuration(1, TimeUnitType.Hour));

Console.WriteLine("Leveling Delay: " + task.Get(Tsk.LevelingDelay));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


