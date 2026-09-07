---
title: "Tsk.Contact"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड. कार्य के लिए जिम्मेदार व्यक्ति का नाम।"
type: docs
weight: 220
url: /hi/net/aspose.tasks/tsk/contact/
---
## Tsk.Contact field

कार्य के लिए जिम्मेदार व्यक्ति का नाम।

```csharp
public static readonly Key<string, TaskKey> Contact;
```

## उदाहरण

Tsk.Contact प्रॉपर्टी को पढ़ने/लिखने का तरीका दिखाता है।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.Contact, "John Smith");

Console.WriteLine("Contact: " + task.Get(Tsk.Contact));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


