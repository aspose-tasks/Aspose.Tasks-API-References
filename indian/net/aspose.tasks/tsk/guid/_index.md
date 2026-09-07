---
title: "Tsk.Guid"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के लिए उत्पन्न अद्वितीय पहचान कोड"
type: docs
weight: 460
url: /hi/net/aspose.tasks/tsk/guid/
---
## Tsk.Guid field

कार्य के लिए उत्पन्न अद्वितीय पहचान कोड।

```csharp
public static readonly Key<string, TaskKey> Guid;
```

## उदाहरण

Tsk.Guid प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Guid, "60648d59-9c2b-4dc6-bfdb-bfd38f331d61");

Console.WriteLine("Guid: " + task.Get(Tsk.Guid));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


