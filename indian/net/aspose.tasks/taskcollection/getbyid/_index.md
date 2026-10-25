---
title: "TaskCollection.GetById"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskCollection मेथड। निर्दिष्ट Id वाला कार्य लौटाता है जिसका पूर्वज इस संग्रह के पैरेंट कार्य है।"
type: docs
weight: 70
url: /hi/net/aspose.tasks/taskcollection/getbyid/
---
## TaskCollection.GetById method

इस संग्रह के पैरेंट टास्क का पूर्वज होने वाले निर्दिष्ट Id वाले टास्क को लौटाता है।

```csharp
public Task GetById(int id)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आईडी | Int32 | TaskEntity Id |

### रिटर्न वैल्यू

वापस करता है [`Task`](../../task/) क्लास का वह उदाहरण जिसका निर्दिष्ट id है और जिसका पूर्वज इस संग्रह का पैरेंट टास्क है।

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

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


