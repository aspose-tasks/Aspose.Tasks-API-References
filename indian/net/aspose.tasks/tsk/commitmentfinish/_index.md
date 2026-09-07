---
title: "Tsk.CommitmentFinish"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। डिलीवरी की समाप्ति तिथि। केवल XML स्वरूप के लिए पढ़ना समर्थित है"
type: docs
weight: 170
url: /hi/net/aspose.tasks/tsk/commitmentfinish/
---
## Tsk.CommitmentFinish field

डिलीवरी की समाप्ति तिथि। केवल XML फ़ॉर्मेट के लिए पढ़ना समर्थित है।

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentFinish;
```

## उदाहरण

दिखाता है कि कैसे Tsk.CommitmentFinish प्रॉपर्टी को पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentFinish, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Finish: " + task.Get(Tsk.CommitmentFinish));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


