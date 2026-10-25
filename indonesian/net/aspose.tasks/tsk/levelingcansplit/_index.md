---
title: "Tsk.LevelingCanSplit"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Tsk field. Menentukan apakah fungsi penyeimbangan sumber daya dapat menyebabkan pemisahan pada pekerjaan yang tersisa pada tugas ini"
type: docs
weight: 760
url: /id/net/aspose.tasks/tsk/levelingcansplit/
---
## Tsk.LevelingCanSplit field

Menentukan apakah fungsi leveling sumber daya dapat menyebabkan pemisahan pada pekerjaan yang tersisa pada tugas ini.

```csharp
public static readonly Key<NullableBool, TaskKey> LevelingCanSplit;
```

## Contoh

Menampilkan cara membaca/menulis properti Tsk.LevelingCanSplit.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task");

task.Set(Tsk.LevelingCanSplit, true);

Console.WriteLine("Leveling Can Split: " + task.Get(Tsk.LevelingCanSplit));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* struct [NullableBool](../../nullablebool/)
* enum [TaskKey](../../taskkey/)
* class [Tsk](../)
* namespace [Aspose.Tasks](../../tsk/)
* assembly [Aspose.Tasks](../../../)


