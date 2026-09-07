---
title: "Task.Clone"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Membuat salinan penuh dari sebuah tugas tanpa subtugas"
type: docs
weight: 1310
url: /id/net/aspose.tasks/task/clone/
---
## Task.Clone method

Membuat salinan penuh dari sebuah tugas tanpa subtugas.

```csharp
public object Clone()
```

### Nilai Kembali

Membuat salinan tugas.

## Contoh

Menampilkan cara menggandakan tugas.

```csharp
var project = new Project();

var originalTask = project.RootTask.Children.Add("Task");
var cloneTask = (Task)originalTask.Clone();

Console.WriteLine("Are tasks equal: " + cloneTask.Equals(originalTask));
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


