---
title: "TaskCollection.Add"
second_title: "Aspose.Tasks .NET के लिए API संदर्भ"
description: "TaskCollection मेथड। निर्दिष्ट टास्क को TaskCollection क्लास के इंस्टेंस में जोड़ता है। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड के उपयोग के बाद Project.Recalculate को कॉल करना चाहिए। यह सभी प्रोजेक्ट टास्क की शुरू/समाप्ति तिथियों को पुनर्निर्धारित करेगा, प्रारंभिक/अंतिम तिथियों को सेट करेगा और स्लैक, कार्य और लागत फ़ील्ड, आईडी और आउटलाइन लेवल जैसे निर्भर फ़ील्ड की गणना करेगा। यदि ParentProject.CalculationMode Manual है तो मेथड केवल टास्क आईडी, आउटलाइन लेवल और आउटलाइन नंबरों की स्वतः गणना करेगा। यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट टास्क को स्वतः पुनर्निर्धारित करेगा (शुरू/समाप्ति तिथियों को सेट करेगा, प्रारंभिक/अंतिम तिथियों को सेट करेगा, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगा, आईडी और आउटलाइन लेवल को पुनः गणना करेगा)।"
type: docs
weight: 50
url: /hi/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

निर्दिष्ट टास्क को [`TaskCollection`](../) क्लास के इंस्टेंस में जोड़ें। यदि ParentProject.CalculationMode None है तो उपयोगकर्ता को इस मेथड के उपयोग के बाद Project.Recalculate() को कॉल करना चाहिए (यह सभी प्रोजेक्ट टास्क को पुनर्निर्धारित करेगा (शुरू/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करेगा) और स्लैक, कार्य और लागत फ़ील्ड, आईडी और आउटलाइन लेवल जैसे निर्भर फ़ील्ड की गणना करेगा)। यदि ParentProject.CalculationMode Manual है तो मेथड केवल टास्क आईडी, आउटलाइन लेवल और आउटलाइन नंबरों की स्वतः गणना करेगा। यदि ParentProject.CalculationMode Automatic है तो मेथड सभी प्रोजेक्ट टास्क को स्वतः पुनर्निर्धारित करेगा (शुरू/समाप्ति तिथियों, प्रारंभिक/अंतिम तिथियों को सेट करेगा, स्लैक, कार्य और लागत फ़ील्ड की गणना करेगा, आईडी और आउटलाइन लेवल को पुनः गणना करेगा)।

```csharp
public void Add(Task item)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| आइटम | कार्य | निर्दिष्ट कार्य जिसे इस कार्य संग्रह में जोड़ा जाना चाहिए। |

## उदाहरण

दिखाता है कि कैसे एक कार्य को दूसरे पैरेंट के अंतर्गत ले जाया जाए।

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// आईडी द्वारा कार्य प्राप्त करें
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// कार्य 6 को दूसरे पैरेंट में जोड़ना
task2.Children.Add(task);
```

### संबंधित देखें

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

पिछले टास्क के समान आउटलाइन लेवल पर प्रोजेक्ट टास्क्स संग्रह में नया टास्क जोड़ता है।

```csharp
public Task Add()
```

### रिटर्न वैल्यू

नए जोड़े गए [`Task`](../../task/) वर्ग की इंस्टेंस लौटाता है।

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

---

## Add(string) {#add_2}

चाइल्ड टास्क्स संग्रह में नया टास्क जोड़ता है।

```csharp
public Task Add(string taskName)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskName | स्ट्रिंग | निर्दिष्ट कार्य नाम। |

### रिटर्न वैल्यू

नए जोड़े गए [`Task`](../../task/) वर्ग की इंस्टेंस लौटाता है।

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

---

## Add(string, int) {#add_3}

चाइल्ड टास्क्स संग्रह में नया आवर्ती टास्क जोड़ता है।

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| taskName | स्ट्रिंग | निर्दिष्ट कार्य नाम। |
| beforeTaskId | Int32 | निर्दिष्ट आईडी वह है जिसके पहले एक नया कार्य डाला जाएगा। |

### रिटर्न वैल्यू

निर्दिष्ट आईडी वाले कार्य से पहले डाले गए कार्य को लौटाता है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentOutOfRangeException | यदि निर्दिष्ट आईडी मान्य कार्य आईडी नहीं है तो ArgumentOutOfRangeException फेंका जाता है। |

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

---

## Add(RecurringTaskParameters) {#add_1}

निर्दिष्ट आईडी वाले टास्क से पहले और समान आउटलाइन लेवल पर नया टास्क सम्मिलित करता है।

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| पैरामीटर | प्रकार | विवरण |
| --- | --- | --- |
| parameters | RecurringTaskParameters | आवर्ती कार्य बनाने के लिए निर्दिष्ट पैरामीटर। |

### रिटर्न वैल्यू

नए जोड़े गए [`Task`](../../task/) वर्ग की इंस्टेंस लौटाता है।

### अपवाद

| अपवाद | शर्त |
| --- | --- |
| ArgumentNullException | यदि निर्दिष्ट पैरामीटर null हों तो फेंका जाता है। |
| ArgumentException | यदि निर्दिष्ट पैरामीटर अमान्य हों तो फेंका जाता है। |

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
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


