---
title: "Prj.NewTaskStartDate"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Bidang Prj. Jenis tanggal mulai default untuk tugas baru"
type: docs
weight: 580
url: /id/net/aspose.tasks/prj/newtaskstartdate/
---
## Prj.NewTaskStartDate field

Jenis tanggal mulai default untuk tugas baru.

```csharp
public static readonly Key<TaskStartDateType, PrjKey> NewTaskStartDate;
```

## Contoh

Menampilkan cara mengatur atribut untuk tugas baru.

```csharp
var project = new Project();
project.Set(Prj.NewTaskStartDate, TaskStartDateType.CurrentDate);

Console.WriteLine("New Task Start Date: " + project.Get(Prj.NewTaskStartDate));
```

### Lihat Juga

* struct [Key&lt;T,K&gt;](../../key-2/)
* enum [TaskStartDateType](../../taskstartdatetype/)
* enum [PrjKey](../../prjkey/)
* class [Prj](../)
* namespace [Aspose.Tasks](../../prj/)
* assembly [Aspose.Tasks](../../../)


