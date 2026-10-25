---
title: "Project.RescheduleUncompletedWorkToStartAfter"
second_title: "Aspose.Tasks for .NET Αναφορά API"
description: "Μέθοδος Project. Αναπρογραμματίζει το ατελές έργο του έργου ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία."
type: docs
weight: 1190
url: /el/net/aspose.tasks/project/rescheduleuncompletedworktostartafter/
---
## RescheduleUncompletedWorkToStartAfter(DateTime) {#rescheduleuncompletedworktostartafter}

Αναπρογραμματίζει την ατελή εργασία του έργου ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μετά | DateTime | Η ημερομηνία μετά την οποία θα αναπρογραμματιστεί το ατελές έργο. |

## Παραδείγματα

Δείχνει πώς να ενημερώσετε το έργο και να αναπρογραμματίσετε το ατελές έργο.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Προσθέστε νέες εργασίες
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Προσθήκη συνδέσμων μεταξύ εργασιών
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Καθυστέρηση μιας ημέρας
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Προσθέστε νέες εργασίες
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Προσθήκη συνδέσμων μεταξύ εργασιών
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Αποθηκεύστε το έργο πριν και μετά την ενημέρωση της εργασίας ως ολοκληρωμένη
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά την ενημέρωση της εργασίας του έργου ως ολοκληρωμένη μόνο για καθορισμένα καθήκοντα
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά την ενημέρωση όλης της εργασίας του έργου ως ολοκληρωμένη
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά τον επαναπρογραμματισμό της μη ολοκληρωμένης εργασίας μόνο για καθορισμένα καθήκοντα
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά τον επαναπρογραμματισμό της μη ολοκληρωμένης εργασίας
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)

---

## RescheduleUncompletedWorkToStartAfter(DateTime, List&lt;Task&gt;) {#rescheduleuncompletedworktostartafter_1}

Αναπρογραμματίζει την ατελή εργασία για μια καθορισμένη λίστα εργασιών ώστε να ξεκινήσει μετά από μια καθορισμένη ημερομηνία.

```csharp
public void RescheduleUncompletedWorkToStartAfter(DateTime after, List<Task> taskCollection)
```

| Παράμετρος | Τύπος | Περιγραφή |
| --- | --- | --- |
| μετά | DateTime | Η ημερομηνία μετά την οποία θα αναπρογραμματιστεί το ατελές έργο. |
| taskCollection | List`1 | Λίστα&lt;Task&gt; των εργασιών για τις οποίες θα επαναπρογραμματιστεί η μη ολοκληρωμένη εργασία. |

## Παραδείγματα

Δείχνει πώς να ενημερώσετε το έργο και να αναπρογραμματίσετε το ατελές έργο.

```csharp
var project = new Project();
project.Set(Prj.StartDate, new DateTime(2014, 1, 27, 8, 0, 0));

// Προσθέστε νέες εργασίες
var task1 = project.RootTask.Children.Add("Task 1");
var task2 = project.RootTask.Children.Add("Task 2");
task2.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task3 = project.RootTask.Children.Add("Task 3");
task3.Set(Tsk.Duration, task2.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task4 = project.RootTask.Children.Add("Task 4");
task4.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task5 = project.RootTask.Children.Add("Task 5");
task5.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));

// Προσθήκη συνδέσμων μεταξύ εργασιών
project.TaskLinks.Add(task1, task2, TaskLinkType.FinishToStart);
var link23 = project.TaskLinks.Add(task2, task3, TaskLinkType.FinishToStart);

// Καθυστέρηση μιας ημέρας
link23.LinkLag = 4800;
project.TaskLinks.Add(task3, task4, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task4, task5, TaskLinkType.FinishToStart);

// Προσθέστε νέες εργασίες
var task6 = project.RootTask.Children.Add("Task 6");
var task7 = project.RootTask.Children.Add("Task 7");
task7.Set(Tsk.Duration, task7.ParentProject.GetDuration(24, TimeUnitType.Hour));
var task8 = project.RootTask.Children.Add("Task 8");
task8.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task9 = project.RootTask.Children.Add("Task 9");
task9.Set(Tsk.Duration, task2.ParentProject.GetDuration(16, TimeUnitType.Hour));
var task10 = project.RootTask.Children.Add("Task 10");

// Προσθήκη συνδέσμων μεταξύ εργασιών
project.TaskLinks.Add(task6, task7, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task7, task8, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task8, task9, TaskLinkType.FinishToStart);
project.TaskLinks.Add(task9, task10, TaskLinkType.FinishToStart);
task6.Set(Tsk.IsManual, true);
task7.Set(Tsk.IsManual, true);
task8.Set(Tsk.IsManual, true);
task9.Set(Tsk.IsManual, true);
task10.Set(Tsk.IsManual, true);

// Αποθηκεύστε το έργο πριν και μετά την ενημέρωση της εργασίας ως ολοκληρωμένη
project.Save(OutDir + "RescheduleUncompletedWork_not updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά την ενημέρωση της εργασίας του έργου ως ολοκληρωμένη μόνο για καθορισμένα καθήκοντα
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false, new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά την ενημέρωση όλης της εργασίας του έργου ως ολοκληρωμένη
project.UpdateProjectWorkAsComplete(new DateTime(2014, 1, 28, 17, 0, 0), false);
project.Save(OutDir + "RescheduleUncompletedWork_updated_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά τον επαναπρογραμματισμό της μη ολοκληρωμένης εργασίας μόνο για καθορισμένα καθήκοντα
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 8, 8, 0, 0), new List<Task> { task10 });
project.Save(OutDir + "RescheduleUncompletedWork_specific_rescheduled_out.xml", SaveFileFormat.Xml);

// Αποθήκευση έργου μετά τον επαναπρογραμματισμό της μη ολοκληρωμένης εργασίας
project.RescheduleUncompletedWorkToStartAfter(new DateTime(2014, 2, 7, 8, 0, 0));
project.Save(OutDir + "RescheduleUncompletedWork_rescheduled_out.xml", SaveFileFormat.Xml);
```

### Δείτε επίσης

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


