---
title: "TaskCollection.Add"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "TaskCollection yöntemi. Belirtilen görevi TaskCollection sınıfının örneğine ekler. ParentProject.CalculationMode None ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate metodunu çağırmalıdır. Bu, tüm proje görevlerinin başlangıç/bitiş tarihlerini yeniden planlayacak, erken/son tarihleri ayarlayacak ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplayacaktır. ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise, yöntem tüm proje görevlerini otomatik olarak yeniden planlayacak (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar)."
type: docs
weight: 50
url: /tr/net/aspose.tasks/taskcollection/add/
---
## Add(Task) {#add_4}

[`TaskCollection`](../) sınıfının örneğine belirtilen görevi ekler. ParentProject.CalculationMode None ise, kullanıcı bu yöntemi kullandıktan sonra Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar) yeniden planlayacak ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplayacaktır). ParentProject.CalculationMode Manual ise, yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode Automatic ise, yöntem tüm projenin görevlerini otomatik olarak yeniden planlayacaktır (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar).

```csharp
public void Add(Task item)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| öğe | Görev | belirtilen görev, bu görev koleksiyonuna eklenmelidir. |

## Örnekler

Bir görevi başka bir üst görevin altına nasıl taşıyacağını gösterir.

```csharp
var project = new Project(DataDir + "MoveTask.mpp") { CalculationMode = CalculationMode.Automatic };

// Görevleri Id'lere göre al
var task = project.RootTask.Children.GetByUid(6);
var task2 = project.RootTask.Children.GetByUid(3);

// Görev 6'yı başka bir üst göreve ekleme
task2.Children.Add(task);
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add() {#add}

Son görevin aynı taslak seviyesinde proje görevleri koleksiyonuna yeni görev ekler.

```csharp
public Task Add()
```

### Dönüş Değeri

yeni eklenen [`Task`](../../task/) sınıfının örneğini döndürür.

## Örnekler

Görev koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// görev koleksiyonu yalnızca okunabilir değildir ve genişletilebilir
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// görevler oluştur
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

// proje görevlerini yazdır
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

// bir görev, koleksiyondan ID ile alınabilir
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// veya UID ile
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// aynı zamanda yinelenen bir görev eklenebilir
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

// bir dizideki ilk görev döndürülür
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// koleksiyon düz bir listeye dönüştürülebilir
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string) {#add_2}

Alt görevler koleksiyonuna yeni bir görev ekler.

```csharp
public Task Add(string taskName)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskName | Dize | belirtilen görev adı. |

### Dönüş Değeri

yeni eklenen [`Task`](../../task/) sınıfının örneğini döndürür.

## Örnekler

Görev koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// görev koleksiyonu yalnızca okunabilir değildir ve genişletilebilir
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// görevler oluştur
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

// proje görevlerini yazdır
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

// bir görev, koleksiyondan ID ile alınabilir
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// veya UID ile
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// aynı zamanda yinelenen bir görev eklenebilir
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

// bir dizideki ilk görev döndürülür
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// koleksiyon düz bir listeye dönüştürülebilir
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(string, int) {#add_3}

Alt görevler koleksiyonuna yeni yinelenen bir görev ekler.

```csharp
public Task Add(string taskName, int beforeTaskId)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| taskName | Dize | belirtilen görev adı. |
| beforeTaskId | Int32 | Yeni bir görevin ekleneceği görevin öncesindeki belirtilen görev kimliği. |

### Dönüş Değeri

belirtilen kimliğe sahip görevin öncesine eklenen bir görevi döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentOutOfRangeException | ArgumentOutOfRangeException, belirtilen kimlik geçerli bir görev kimliği değilse fırlatılır. |

## Örnekler

Görev koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// görev koleksiyonu yalnızca okunabilir değildir ve genişletilebilir
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// görevler oluştur
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

// proje görevlerini yazdır
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

// bir görev, koleksiyondan ID ile alınabilir
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// veya UID ile
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// aynı zamanda yinelenen bir görev eklenebilir
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

// bir dizideki ilk görev döndürülür
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// koleksiyon düz bir listeye dönüştürülebilir
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)

---

## Add(RecurringTaskParameters) {#add_1}

Belirtilen kimliğe (id) sahip görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler.

```csharp
public Task Add(RecurringTaskParameters parameters)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| parameters | RecurringTaskParameters | Yinelenen görev oluşturmak için belirtilen parametreler. |

### Dönüş Değeri

yeni eklenen [`Task`](../../task/) sınıfının örneğini döndürür.

### İstisnalar

| istisna | koşul |
| --- | --- |
| ArgumentNullException | Belirtilen parametreler null ise fırlatılır. |
| ArgumentException | Belirtilen parametreler geçersiz ise fırlatılır. |

## Örnekler

Görev koleksiyonlarıyla nasıl çalışılacağını gösterir.

```csharp
var project = new Project();

// görev koleksiyonu yalnızca okunabilir değildir ve genişletilebilir
Console.WriteLine("Is task collection read - only: " + project.RootTask.Children.IsReadOnly);

// görevler oluştur
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

// proje görevlerini yazdır
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

// bir görev, koleksiyondan ID ile alınabilir
var task1ToEdit = project.RootTask.Children.GetById(1);
task1ToEdit.Set(Tsk.Name, "Task 1 (Edited)");

// veya UID ile
var taskToEdit2 = project.RootTask.Children.GetByUid(2);
taskToEdit2.Set(Tsk.Name, "Task 2 (Edited)");

// aynı zamanda yinelenen bir görev eklenebilir
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

// bir dizideki ilk görev döndürülür
var recurring = project.RootTask.Children.Add(parameters);
Console.WriteLine("Task name: " + recurring.Get(Tsk.Name));

// koleksiyon düz bir listeye dönüştürülebilir
List<Task> tasks = project.RootTask.Children.ToList();
foreach (var task in tasks)
{
    task.Delete();
}
```

### Ayrıca Bakınız

* class [Task](../../task/)
* class [RecurringTaskParameters](../../recurringtaskparameters/)
* class [TaskCollection](../)
* namespace [Aspose.Tasks](../../taskcollection/)
* assembly [Aspose.Tasks](../../../)


