---
title: "Tsk.Duration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। कार्य के सक्रिय कार्य समय की कुल अवधि, जिसे दर्ज किया गया है या माइक्रोसॉफ्ट प्रोजेक्ट द्वारा शुरू तिथि, समाप्ति तिथि, कैलेंडर और अन्य शेड्यूलिंग कारकों के आधार पर गणना किया गया है"
type: docs
weight: 300
url: /hi/net/aspose.tasks/tsk/duration/
---
## Tsk.Duration field

कार्य के लिए सक्रिय कार्य समय की कुल अवधि, जो दर्ज की गई या Microsoft Project द्वारा प्रारंभ तिथि, समाप्ति तिथि, कैलेंडर और अन्य शेड्यूलिंग कारकों के आधार पर गणना की गई हो।

```csharp
public static readonly Key<Duration, TaskKey> Duration;
```

## उदाहरण

दिखाता है कि कार्य की अवधि कैसे सेट करें।

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddTaskDuration_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


