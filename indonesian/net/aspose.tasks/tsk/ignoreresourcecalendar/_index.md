---
title: "Tsk.IgnoreResourceCalendar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah penjadwalan tugas mempertimbangkan kalender sumber daya yang ditugaskan ke tugas tersebut"
type: docs
weight: 530
url: /id/net/aspose.tasks/tsk/ignoreresourcecalendar/
---
## Tsk.IgnoreResourceCalendar field

Menentukan apakah penjadwalan tugas mempertimbangkan kalender sumber daya yang ditugaskan ke tugas tersebut.

```csharp
public static readonly Key<NullableBool, TaskKey> IgnoreResourceCalendar;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.IgnoreResourceCalendar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.IgnoreResourceCalendar, true);

Console.WriteLine("Ignore Resource Calendar: " + task.Get(Tsk.IgnoreResourceCalendar));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


