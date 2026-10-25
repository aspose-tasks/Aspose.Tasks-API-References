---
title: "Tsk.HideBar"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Tsk. Menentukan apakah bar Gantt dari sebuah tugas disembunyikan saat ditampilkan di Microsoft Project."
type: docs
weight: 480
url: /id/net/aspose.tasks/tsk/hidebar/
---
## Tsk.HideBar field

Menentukan apakah bar Gantt dari sebuah tugas disembunyikan saat ditampilkan di Microsoft Project.

```csharp
public static readonly Key<NullableBool, TaskKey> HideBar;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.HideBar.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.HideBar, true);

Console.WriteLine("Hide Bar: " + task.Get(Tsk.HideBar));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


