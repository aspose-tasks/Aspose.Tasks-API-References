---
title: "Tsk.LevelingCanSplit"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि क्या संसाधन लेवलिंग फ़ंक्शन इस कार्य पर शेष कार्य में विभाजन कर सकता है"
type: docs
weight: 760
url: /hi/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

निर्धारित करता है कि संसाधन लेवलिंग फ़ंक्शन इस कार्य के शेष कार्य पर विभाजन कर सकता है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## उदाहरण

Tsk.LevelingCanSplit प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


