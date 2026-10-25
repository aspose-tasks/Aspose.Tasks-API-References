---
title: "Tsk.StatusManager"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। उस एंटरप्राइज़ संसाधन का नाम जो वर्तमान कार्य के लिए संसाधनों से स्थिति अपडेट प्राप्त करेगा"
type: docs
weight: 1050
url: /hi/net/aspose.tasks/tsk/statusmanager/
---
## Tsk.StatusManager field

वर्तमान कार्य के लिए संसाधनों से स्थिति अपडेट प्राप्त करने वाले एंटरप्राइज़ संसाधन का नाम।

```csharp
public static readonly Key<string, TaskKey> StatusManager;
```

## उदाहरण

दिखाता है कि Tsk.StatusManager प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.StatusManager, "John Smith");

Console.WriteLine("Status Manager: " + task.Get(Tsk.StatusManager));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


