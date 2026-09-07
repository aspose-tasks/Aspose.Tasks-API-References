---
title: "Tsk.IsNull"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि कार्य एक null कार्य है या नहीं"
type: docs
weight: 640
url: /hi/net/aspose.tasks/tsk/isnull/
---
## Tsk.IsNull field

निर्धारित करता है कि कार्य एक शून्य कार्य है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IsNull;
```

## उदाहरण

दिखाता है कि Tsk.IsNull प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsNull, true);

Console.WriteLine("Is Null: " + task.Get(Tsk.IsNull));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


