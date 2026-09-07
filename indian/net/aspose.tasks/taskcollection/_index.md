---
title: "क्लास TaskCollection"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "Aspose.Tasks.TaskCollection क्लास। Task ऑब्जेक्ट्स का एक संग्रह दर्शाता है"
type: docs
weight: 2390
url: /hi/net/aspose.tasks/taskcollection/
---
## TaskCollection class

[`Task`](../task/) ऑब्जेक्ट्स का संग्रह दर्शाता है।

```csharp
public class TaskCollection : IList<Task>
```

## गुण

| नाम | विवरण |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | TaskCollection में शामिल ऑब्जेक्ट्स की संख्या प्राप्त करता है। |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | एक मान प्राप्त करता है जो दर्शाता है कि यह संग्रह केवल-पढ़ने योग्य है या नहीं। |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | निर्दिष्ट इंडेक्स पर तत्व लौटाता है। |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | TaskCollection ऑब्जेक्ट के पैरेंट प्रोजेक्ट को प्राप्त करता है। |

## विधियाँ

| नाम | विवरण |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | पिछले टास्क के समान आउटलाइन लेवल पर प्रोजेक्ट टास्क्स संग्रह में नया टास्क जोड़ता है। |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | निर्दिष्ट आईडी वाले टास्क से पहले और समान आउटलाइन लेवल पर नया टास्क सम्मिलित करता है। |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | चाइल्ड टास्क्स संग्रह में नया टास्क जोड़ता है। |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | निर्दिष्ट टास्क को `TaskCollection` क्लास के इंस्टेंस में जोड़ें। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड का उपयोग करने के बाद Project.Recalculate() को कॉल करना चाहिए (यह सभी प्रोजेक्ट टास्क्स को पुनः शेड्यूल करेगा (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगा) और स्लैक, कार्य और लागत फ़ील्ड, आईडी और आउटलाइन लेवल जैसे निर्भर फ़ील्ड की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो मेथड केवल टास्क आईडी, आउटलाइन लेवल और आउटलाइन नंबर स्वचालित रूप से गणना करेगा। यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट टास्क्स को स्वचालित रूप से पुनः शेड्यूल करेगा (शुरू/समाप्ति तिथियां, प्रारंभिक/अंतिम तिथियां सेट करेगा, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगा, आईडी और आउटलाइन लेवल को पुनः गणना करेगा)। |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | चाइल्ड टास्क्स संग्रह में नया आवर्ती टास्क जोड़ता है। |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | जांचता है कि संग्रह में निर्दिष्ट आइटम मौजूद है या नहीं। |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | इस संग्रह के पैरेंट टास्क का पूर्वज होने वाले निर्दिष्ट Id वाले टास्क को लौटाता है। |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | इस संग्रह के पैरेंट टास्क का पूर्वज होने वाले निर्दिष्ट Uid वाले टास्क को लौटाता है। |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | इस संग्रह के लिए एक एन्यूमरेटर लौटाता है। |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | यह IList की Insert मेथड का स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकता है। |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | यह ICollection की Remove मेथड का स्टब इम्प्लीमेंटेशन है, जो केवल NotSupportedException फेंकता है। |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | TaskCollection ऑब्जेक्ट को [`Task`](../task/) ऑब्जेक्ट्स की सूची में परिवर्तित करता है। |

## उदाहरण

टास्क कलेक्शन्स के साथ काम करने का तरीका दिखाता है।

```csharp
var project = new Project();

// टास्क कलेक्शन रीड-ओनली नहीं है और इसे विस्तारित किया जा सकता है।
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// टास्क बनाएं
var task1 = project.RootTask.Children.Add();
task1.Set(Tsk.Name, "Task 1");
task1.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task1.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task1.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task3.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));
task3.Set(Tsk.Finish, new DateTime(2020, 4, 15, 17, 0, 0));
var task2 = project.RootTask.Children.Add("Task 2", 2);
task2.Set(Tsk.Start, new DateTime(2020, 4, 15, 8, 0, 0));
task2.Set(Tsk.Duration, project.GetDuration(1, TimeUnitType.Day));

// प्रोजेक्ट टास्क्स प्रिंट करें
Console.WriteLine("Count of tasks: " + project.RootTask.Children.Count);
foreach (var child in project.RootTask.Children)
{
    Console.WriteLine("Parent Project: " + project.RootTask.ParentProject.Get(Prj.Name));
    Console.WriteLine("Task name: " + child.Get(Tsk.Name));
    Console.WriteLine("Task start: " + child.Get(Tsk.Start));
    Console.WriteLine("Task duration: " + child.Get(Tsk.Duration));
    Console.WriteLine("Task finish: " + child.Get(Tsk.Finish));
    Console.WriteLine();
}

// एक टास्क को आईडी द्वारा संग्रह से लिया जा सकता है।
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// या UID द्वारा
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// आप भी एक आवर्ती टास्क जोड़ सकते हैं
var parameters = new RecurringTaskParameters
                     {
                         TaskName = "t1",
                         Duration = project.GetDuration(1, TimeUnitType.Day),
                         RecurrencePattern = new DailyRecurrencePattern
                                                 {
                                                     Repetition = new DailyCalendarRepetition { RepetitionInterval = 1 },
                                                     RecurrenceRange = new EndByRecurrenceRange
                                                                           {
                                                                               Start = new DateTime(2020, 4, 13, 8, 0, 0),
                                                                               Finish = new DateTime(2021, 4, 13, 17, 0, 0)
                                                                           }
                                                 }
                     };

// एक क्रम में पहला टास्क लौटाया जाता है।
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// संग्रह को साधारण सूची में परिवर्तित किया जा सकता है।
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### संबंधित देखें

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


