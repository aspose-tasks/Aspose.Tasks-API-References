---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। निर्धारित करता है कि कार्य की समय-सारणी में कार्य को सौंपे गए संसाधनों के कैलेंडर को ध्यान में रखा गया है या नहीं"
type: docs
weight: 530
url: /hi/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

निर्धारित करता है कि कार्य का शेड्यूलिंग कार्य को सौंपे गए संसाधनों के कैलेंडर को ध्यान में रखता है या नहीं।

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## उदाहरण

दिखाता है कि Tsk.IgnoreResourceCalendar प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


