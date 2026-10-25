---
title: "Tsk.IsSubprojectReadOnly"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। यह निर्धारित करता है कि उप‑प्रोजेक्ट केवल‑पढ़ने योग्य है या नहीं"
type: docs
weight: 710
url: /hi/net/aspose.tasks/tsk/issubprojectreadonly/
---
## Tsk.IsSubprojectReadOnly field

निर्धारित करता है कि उपप्रोजेक्ट केवल-पढ़ने योग्य है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsSubprojectReadOnly;
```

## उदाहरण

दिखाता है कि Tsk.IsSubprojectReadOnly प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsSubprojectReadOnly, true);

Console.WriteLine("Is Subproject Read Only: " + task.Get(Tsk.IsSubprojectReadOnly));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


