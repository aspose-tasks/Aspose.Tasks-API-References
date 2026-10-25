---
title: "Tsk.PreleveledStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk field. संसाधन स्तरन किए जाने से पहले कार्य की प्रारंभ तिथि"
type: docs
weight: 920
url: /hi/net/aspose.tasks/tsk/preleveledstart/
---
## Tsk.PreleveledStart field

संसाधन लेवलिंग करने से पहले कार्य की प्रारंभ तिथि।

```csharp
public static readonly Key<DateTime, TaskKey> PreleveledStart;
```

## उदाहरण

दिखाता है कि कैसे Tsk.PreleveledStart प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PreleveledStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Preleveled Start: " + task.Get(Tsk.PreleveledStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


