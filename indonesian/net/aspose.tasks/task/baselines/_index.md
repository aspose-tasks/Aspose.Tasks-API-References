---
title: "Task.Baselines"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan atau mengatur koleksi nilai baseline dari tugas"
type: docs
weight: 130
url: /id/net/aspose.tasks/task/baselines/
---
## Task.Baselines property

Mendapatkan atau mengatur koleksi nilai baseline tugas.

```csharp
public TaskBaselineCollection Baselines { get; set; }
```

## Contoh

Menunjukkan cara membaca baseline tugas.

```csharp
var project = new Project();

// tetapkan baseline
var task = project.RootTask.Children.Add("Task");
project.SetBaseline(BaselineType.Baseline);

// Tampilkan durasi baseline tugas
foreach (var baseline in task.Baselines)
{
    Console.WriteLine("Baseline duration is 1 day: {0}", baseline.Duration.ToString().Equals("1 day"));
    Console.WriteLine("BaselineStart is same as Task Start: {0}", baseline.Start.Equals(task.Get(Tsk.Start)));
    Console.WriteLine("BaselineFinish is same as Task Finish: {0}", baseline.Finish.Equals(task.Get(Tsk.Finish)));
}
```

### Lihat Juga

* class [TaskBaselineCollection](../../taskbaselinecollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


