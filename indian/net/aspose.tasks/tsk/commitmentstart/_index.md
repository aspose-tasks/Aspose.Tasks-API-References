---
title: "Tsk.CommitmentStart"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। डिलीवरी की प्रारंभ तिथि। पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है"
type: docs
weight: 180
url: /hi/net/aspose.tasks/tsk/commitmentstart/
---
## Tsk.CommitmentStart field

डिलीवरी की प्रारंभ तिथि। केवल XML फ़ॉर्मेट के लिए पढ़ना समर्थित है।

```csharp
public static readonly Key<DateTime, TaskKey> CommitmentStart;
```

## उदाहरण

दिखाता है कि Tsk.CommitmentStart प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentStart, new DateTime(2020, 4, 10, 8, 0, 0));

Console.WriteLine("Commitment Start: " + task.Get(Tsk.CommitmentStart));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


