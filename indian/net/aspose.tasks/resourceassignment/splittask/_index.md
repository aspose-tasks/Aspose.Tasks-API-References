---
title: "ResourceAssignment.SplitTask"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। कार्य को दो भागों में विभाजित करता है।"
type: docs
weight: 770
url: /hi/net/aspose.tasks/resourceassignment/splittask/
---
## ResourceAssignment.SplitTask method

कार्य को दो भागों में विभाजित करता है।

```csharp
public void SplitTask(DateTime start, DateTime finish, Calendar calendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| प्रारंभ | DateTime | विभाजन के आधार पर कार्य व्यवधान की शुरुआत। |
| समाप्ति | DateTime | विभाजन के आधार पर कार्य व्यवधान का अंत। |
| कैलेंडर | कैलेंडर | विभाजन के आधार पर कैलेंडर। |

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentOutOfRangeException | जब प्रारंभ तिथि असाइनमेंट की प्रारंभ तिथि से कम हो तो थ्रो करता है। |
| ArgumentOutOfRangeException | जब समाप्ति तिथि असाइनमेंट की समाप्ति तिथि से अधिक हो तो थ्रो करता है। |

## उदाहरण

एक कार्य के लिए विभाजन जोड़ने का तरीका दिखाता है।

```csharp
var project = new Project();

// एक मानक कैलेंडर प्राप्त करें
var calendar = project.Get(Prj.Calendar);

// परियोजना के कैलेंडर सेटिंग्स सेट करें
project.Set(Prj.StartDate, new DateTime(2000, 3, 15, 8, 0, 0));
project.Set(Prj.FinishDate, new DateTime(2000, 4, 21, 17, 0, 0));

// रूट टास्क में एक नया कार्य जोड़ें
var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Duration, project.GetDuration(3));

// एक नया रिसोर्स असाइनमेंट बनाएं और टाइम‑फेज़्ड डेटा उत्पन्न करें
var assignment = project.ResourceAssignments.Add(task, null);
assignment.TimephasedDataFromTaskDuration(calendar);

// कार्य को 3 भागों में विभाजित करें।
// स्प्लिट के लिए उपयोग किए जाने वाले SplitTask मेथड को प्रारंभ तिथि और समाप्ति तिथि के आर्ग्युमेंट प्रदान करें
assignment.SplitTask(new DateTime(2000, 3, 16, 8, 0, 0), new DateTime(2000, 3, 16, 17, 0, 0), calendar);
assignment.SplitTask(new DateTime(2000, 3, 18, 8, 0, 0), new DateTime(2000, 3, 18, 17, 0, 0), calendar);
assignment.Set(Asn.WorkContour, WorkContourType.Contoured);

project.Save(OutDir + "CreateSplitTasks_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Calendar](../../calendar/)
* class [ResourceAssignment](../)
* namespace [Aspose.Tasks](../../resourceassignment/)
* assembly [Aspose.Tasks](../../../)


