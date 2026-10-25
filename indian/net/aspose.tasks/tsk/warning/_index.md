---
title: "Tsk.Warning"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। वह फ़्लैग दर्शाता है जो संकेत करता है कि कार्य में समय‑सारणी में विसंगतियाँ हैं"
type: docs
weight: 1120
url: /hi/net/aspose.tasks/tsk/warning/
---
## Tsk.Warning field

फ़्लैग जो संकेत करता है कि कार्य में अनुसूची विसंगतियां हैं।

```csharp
public static readonly Key<bool, TaskKey> Warning;
```

## उदाहरण

एक कार्य चेतावनी को पढ़ने का तरीका दिखाता है।

```csharp
var project = new Project(DataDir + "schedule-conflict.mpp");
var task = project.RootTask.Children.GetById(1);
Console.WriteLine(task.Get(Tsk.Warning));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


