---
title: "Tsk.IgnoreWarnings"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। दर्शाता है कि Microsoft Project में शेड्यूल टकराव चेतावनी संकेतक को छिपाना है या नहीं"
type: docs
weight: 540
url: /hi/net/aspose.tasks/tsk/ignorewarnings/
---
## Tsk.IgnoreWarnings field

यह दर्शाता है कि Microsoft Project में शेड्यूल संघर्ष चेतावनी संकेतक को छिपाना है या नहीं।

```csharp
public static readonly Key<bool, TaskKey> IgnoreWarnings;
```

## उदाहरण

दिखाता है कि Tsk.IgnoreWarnings प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreWarnings, true);

Console.WriteLine("Ignore Warnings: " + task.Get(Tsk.IgnoreWarnings));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


