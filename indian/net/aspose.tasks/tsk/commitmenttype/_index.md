---
title: "Tsk.CommitmentType"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि क्या किसी कार्य का संबंधित डिलीवरी है या उस डिलीवरी पर निर्भरता है। पढ़ना केवल XML फ़ॉर्मेट के लिए समर्थित है"
type: docs
weight: 190
url: /hi/net/aspose.tasks/tsk/commitmenttype/
---
## Tsk.CommitmentType field

निर्धारित करता है कि क्या टास्क का कोई संबंधित डिलीवरी है या संबंधित डिलीवरी पर निर्भरता है। केवल XML फ़ॉर्मेट के लिए पढ़ना समर्थित है।

```csharp
public static readonly Key<int, TaskKey> CommitmentType;
```

## उदाहरण

दिखाता है कि Tsk.CommitmentType प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.CommitmentType, 2);

Console.WriteLine("Commitment Type: " + task.Get(Tsk.CommitmentType));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


