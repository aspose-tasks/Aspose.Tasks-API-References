---
title: "Tsk.IsActive"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि कार्य सक्रिय है या नहीं। निष्क्रिय कार्य अब अन्य कार्यों या समग्र प्रोजेक्ट शेड्यूल को प्रभावित नहीं करते।"
type: docs
weight: 550
url: /hi/net/aspose.tasks/tsk/isactive/
---
## Tsk.IsActive field

निर्धारित करता है कि कार्य सक्रिय है या नहीं। निष्क्रिय कार्य अब अन्य कार्यों या समग्र प्रोजेक्ट शेड्यूल को प्रभावित नहीं करते।

```csharp
public static readonly Key<NullableBool, TaskKey> IsActive;
```

## उदाहरण

दिखाता है कि Tsk.IsActive प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IsActive, true);

Console.WriteLine("Is Active: " + task.Get(Tsk.IsActive));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


