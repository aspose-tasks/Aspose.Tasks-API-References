---
title: "Project.UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Project मेथड। पूरे प्रोजेक्ट के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है।"
type: docs
weight: 1270
url: /hi/net/aspose.tasks/project/updateprojectworkascomplete/
---
## UpdateProjectWorkAsComplete(DateTime, bool) {#updateprojectworkascomplete}

पूरी परियोजना के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है।

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| completeThrough | DateTime | कार्य को पूर्ण के रूप में अपडेट करने की तिथि। |
| setZeroOrHundredPercentCompleteOnly | Boolean | यदि true पर सेट किया गया है, तो केवल उन कार्यों को 100% पूर्ण के रूप में अपडेट करता है जिनकी समाप्ति तिथि निर्दिष्ट complete-through तिथि से पहले है। अन्यथा, निर्धारित प्रारंभ और complete-through तिथियों के आधार पर प्रतिशत पूर्ण मान की गणना करता है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को कैसे अपडेट करें और अपूर्ण कार्य को पुनर्निर्धारित करें।

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// नए कार्य जोड़ें।
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// कार्य के बीच लिंक जोड़ें
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// एक दिन की देरी
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// नए कार्य जोड़ें।
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// कार्य के बीच लिंक जोड़ें
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// काम को पूर्ण के रूप में अपडेट करने से पहले और बाद में प्रोजेक्ट सहेजें
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// निर्दिष्ट कार्यों के लिए केवल प्रोजेक्ट कार्य को पूर्ण के रूप में अपडेट करने के बाद प्रोजेक्ट सहेजें
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// सभी प्रोजेक्ट कार्य को पूर्ण के रूप में अपडेट करने के बाद प्रोजेक्ट सहेजें
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// निर्दिष्ट कार्यों के लिए केवल अपूर्ण कार्य को पुनः निर्धारित करने के बाद प्रोजेक्ट सहेजें
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// अपूर्ण कार्य को पुनः निर्धारित करने के बाद प्रोजेक्ट सहेजें
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## UpdateProjectWorkAsComplete(DateTime, bool, List&lt;Task&gt;) {#updateprojectworkascomplete_1}

निर्दिष्ट कार्यों की सूची के लिए निर्दिष्ट तिथि तक सभी कार्य को पूर्ण के रूप में अपडेट करता है।

```csharp
public void UpdateProjectWorkAsComplete(DateTime completeThrough, 
    bool setZeroOrHundredPercentCompleteOnly, List<Task> taskCollection)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| completeThrough | DateTime | कार्य को पूर्ण के रूप में अपडेट करने की तिथि। |
| setZeroOrHundredPercentCompleteOnly | Boolean | यदि true पर सेट किया गया है, तो केवल उन कार्यों को 100% पूर्ण के रूप में अपडेट करता है जिनकी समाप्ति तिथि निर्दिष्ट complete-through तिथि से पहले है। अन्यथा, निर्धारित प्रारंभ और complete-through तिथियों के आधार पर प्रतिशत पूर्ण मान की गणना करता है। |
| taskCollection | List`1 | List&lt;Task&gt; उन कार्यों की सूची जिनके लिए कार्य को अपडेट किया जाना है। |

## उदाहरण

दिखाता है कि प्रोजेक्ट को कैसे अपडेट करें और अपूर्ण कार्य को पुनर्निर्धारित करें।

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// नए कार्य जोड़ें।
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// कार्य के बीच लिंक जोड़ें
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// एक दिन की देरी
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// नए कार्य जोड़ें।
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// कार्य के बीच लिंक जोड़ें
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// काम को पूर्ण के रूप में अपडेट करने से पहले और बाद में प्रोजेक्ट सहेजें
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// निर्दिष्ट कार्यों के लिए केवल प्रोजेक्ट कार्य को पूर्ण के रूप में अपडेट करने के बाद प्रोजेक्ट सहेजें
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// सभी प्रोजेक्ट कार्य को पूर्ण के रूप में अपडेट करने के बाद प्रोजेक्ट सहेजें
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// निर्दिष्ट कार्यों के लिए केवल अपूर्ण कार्य को पुनः निर्धारित करने के बाद प्रोजेक्ट सहेजें
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// अपूर्ण कार्य को पुनः निर्धारित करने के बाद प्रोजेक्ट सहेजें
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### संबंधित देखें

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


