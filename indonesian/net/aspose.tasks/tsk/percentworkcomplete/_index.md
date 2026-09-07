---
title: "Tsk.PercentWorkComplete"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Status terkini sebuah tugas yang dinyatakan sebagai persentase pekerjaan yang telah selesai"
type: docs
weight: 890
url: /id/net/aspose.tasks/tsk/percentworkcomplete/
---
## Tsk.PercentWorkComplete field

Status terkini tugas dinyatakan sebagai persentase pekerjaan yang telah selesai.

```csharp
public static readonly Key<int, TaskKey> PercentWorkComplete;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.PercentWorkComplete.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.PercentWorkComplete, 10);

Console.WriteLine("Percent Work Complete: " + task.Get(Tsk.PercentWorkComplete));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


