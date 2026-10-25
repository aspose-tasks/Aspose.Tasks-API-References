---
title: "Tsk.ActualOvertimeWork"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Tsk फ़ील्ड। उन संसाधनों द्वारा कार्यों को सौंपे जाने पर पहले से किए गए ओवरटाइम कार्य की वास्तविक मात्रा"
type: docs
weight: 60
url: /hi/net/aspose.tasks/tsk/actualovertimework/
---
## Tsk.ActualOvertimeWork field

टास्क को सौंपे गए संसाधनों द्वारा पहले से किए गए ओवरटाइम कार्य की वास्तविक मात्रा।

```csharp
public static readonly Key<Duration, TaskKey> ActualOvertimeWork;
```

## उदाहरण

दिखाता है कि Tsk.ActualOvertimeWork प्रॉपर्टी को कैसे पढ़ें/लिखें।

```csharp
var project = new Project();
project.Set(Prj.WorkFormat, TimeUnitType.Day);

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeWork, project.GetWork(1));

Console.WriteLine("Actual Overtime Work: " + task.Get(Tsk.ActualOvertimeWork));
```

### संबंधित देखें

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [Duration](../../duration/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


