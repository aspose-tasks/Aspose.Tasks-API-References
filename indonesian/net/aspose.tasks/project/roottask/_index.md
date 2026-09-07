---
title: "Project.RootTask"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Project. Mendapatkan akar dari pohon tugas"
type: docs
weight: 800
url: /id/net/aspose.tasks/project/roottask/
---
## Project.RootTask property

Mendapatkan akar dari pohon tugas.

```csharp
public Task RootTask { get; }
```

## Contoh

Menampilkan cara menambahkan tugas ke dalam proyek dengan menggunakan tugas akar proyek.

```csharp
var project = new Project();

var task = project.RootTask.Children.Add("Task1");
task.Set(Tsk.Start, new DateTime(2012, 8, 23, 8, 0, 0));
task.Set(Tsk.Duration, project.GetDuration(24, TimeUnitType.Hour));
task.Set(Tsk.ActualStart, new DateTime(2012, 8, 23, 8, 0, 0));

project.Save(OutDir + "AddNewTask_out.xml", SaveFileFormat.Xml);
```

### Lihat Juga

* class [Task](../../task/)
* class [Project](../)
* namespace [Aspose.Tasks](../../project/)
* assembly [Aspose.Tasks](../../../)


