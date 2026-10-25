---
title: "ResourceAssignment.TimephasedDataFromTaskDuration"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "ResourceAssignment मेथड। कार्य अवधि और निर्धारित प्रारंभ तिथि के आधार पर समय‑फेज़्ड डेटा की सूची उत्पन्न करता है।"
type: docs
weight: 780
url: /hi/net/aspose.tasks/resourceassignment/timephaseddatafromtaskduration/
---
## ResourceAssignment.TimephasedDataFromTaskDuration method

कार्य की अवधि और निर्धारित प्रारंभ तिथि के आधार पर टाइम‑फ़ेज़्ड डेटा की सूची उत्पन्न करता है।

```csharp
public void TimephasedDataFromTaskDuration(Calendar calendar)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| कैलेंडर | कैलेंडर | समय‑फेज़्ड डेटा उत्पन्न करने के लिए कैलेंडर। |

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


