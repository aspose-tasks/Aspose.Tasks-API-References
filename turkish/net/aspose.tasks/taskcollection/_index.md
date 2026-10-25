---
title: "Sınıf TaskCollection"
second_title: "Aspose.Tasks for .NET API Referansı"
description: "Aspose.Tasks.TaskCollection sınıfı. Task nesnelerinin bir koleksiyonunu temsil eder"
type: docs
weight: 2390
url: /tr/net/aspose.tasks/taskcollection/
---
## TaskCollection class

[`Task`](../task/) nesnelerinin bir koleksiyonunu temsil eder.

```csharp
public class TaskCollection : IList<Task>
```

## Özellikler

| Ad | Açıklama |
| --- | --- |
| [Count](../../aspose.tasks/taskcollection/count/) { get; } | TaskCollection içinde bulunan nesne sayısını alır. |
| [IsReadOnly](../../aspose.tasks/taskcollection/isreadonly/) { get; } | Bu koleksiyonun yalnızca okunabilir olup olmadığını gösteren bir değeri alır. |
| [Item](../../aspose.tasks/taskcollection/item/) { get; set; } | Belirtilen indeksteki öğeyi döndürür. |
| [ParentProject](../../aspose.tasks/taskcollection/parentproject/) { get; } | TaskCollection nesnesinin üst projesini alır. |

## Yöntemler

| Ad | Açıklama |
| --- | --- |
| [Add](../../aspose.tasks/taskcollection/add/#add)() | Son görevin aynı taslak seviyesinde proje görevleri koleksiyonuna yeni görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_1)(RecurringTaskParameters) | Belirtilen kimliğe (id) sahip görevin önüne ve aynı taslak seviyesinde yeni bir görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_2)(string) | Alt görevler koleksiyonuna yeni bir görev ekler. |
| [Add](../../aspose.tasks/taskcollection/add/#add_4)(Task) | `TaskCollection` sınıfının örneğine belirtilen görevi ekleyin. ParentProject.CalculationMode değeri None ise, bu yöntemi kullandıktan sonra kullanıcı Project.Recalculate() metodunu çağırmalıdır (Bu, tüm proje görevlerini (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar) yeniden zamanlayacak ve gecikmeler, iş ve maliyet alanları, kimlikler ve taslak seviyeleri gibi bağımlı alanları hesaplayacaktır). ParentProject.CalculationMode değeri Manual ise yöntem yalnızca görev kimliğini, taslak seviyesini ve taslak numaralarını otomatik olarak hesaplayacaktır. ParentProject.CalculationMode değeri Automatic ise yöntem tüm projenin görevlerini otomatik olarak yeniden zamanlayacaktır (başlangıç/bitiş tarihleri, erken/son tarihleri ayarlar, gecikmeleri, işi ve maliyet alanlarını hesaplar, kimlikleri ve taslak seviyelerini yeniden hesaplar). |
| [Add](../../aspose.tasks/taskcollection/add/#add_3)(string, int) | Alt görevler koleksiyonuna yeni yinelenen bir görev ekler. |
| [Contains](../../aspose.tasks/taskcollection/contains/)(Task) | Koleksiyonun belirtilen öğeyi içerip içermediğini kontrol eder. |
| [GetById](../../aspose.tasks/taskcollection/getbyid/)(int) | Bu koleksiyonun üst görevi olan ve belirtilen Id'ye sahip bir görevi döndürür. |
| [GetByUid](../../aspose.tasks/taskcollection/getbyuid/)(int) | Bu koleksiyonun üst görevi olan ve belirtilen Uid'ye sahip bir görevi döndürür. |
| [GetEnumerator](../../aspose.tasks/taskcollection/getenumerator/)() | Bu koleksiyon için bir enumerator döndürür. |
| [Insert](../../aspose.tasks/taskcollection/insert/)(int, Task) | Bu, IList'in Insert metodunun taslak (stub) uygulamasıdır ve yalnızca NotSupportedException fırlatır. |
| [Remove](../../aspose.tasks/taskcollection/remove/)(Task) | Bu, ICollection'ın Remove metodunun taslak (stub) uygulamasıdır ve yalnızca NotSupportedException fırlatır. |
| [ToList](../../aspose.tasks/taskcollection/tolist/)() | TaskCollection nesnesini [`Task`](../task/) nesnelerinden oluşan bir listeye dönüştürür. |

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

* class [Task](../task/)
* namespace [Aspose.Tasks](../../aspose.tasks/)
* assembly [Aspose.Tasks](../../)


