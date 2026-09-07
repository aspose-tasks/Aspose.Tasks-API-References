---
title: "Tsk.ActualOvertimeCost"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Biaya yang timbul untuk kerja lembur yang sudah dilakukan pada tugas oleh sumber daya yang ditugaskan"
type: docs
weight: 50
url: /id/net/aspose.tasks/tsk/actualovertimecost/
---
## Tsk.ActualOvertimeCost field

Biaya yang timbul untuk pekerjaan lembur yang sudah dilakukan pada tugas oleh sumber daya yang ditugaskan.

```csharp
public static readonly Key<decimal, TaskKey> ActualOvertimeCost;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.ActualOvertimeCost.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.ActualOvertimeCost, 10m);

Console.WriteLine("Actual Overtime Cost: " + task.Get(Tsk.ActualOvertimeCost));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


