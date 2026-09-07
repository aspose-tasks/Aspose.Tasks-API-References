---
title: "Task.SplitParts"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Properti Task. Mendapatkan koleksi SplitPart yang mewakili bagian-bagian dari sebuah tugas"
type: docs
weight: 1110
url: /id/net/aspose.tasks/task/splitparts/
---
## Task.SplitParts property

Mendapatkan koleksi SplitPart yang mewakili bagian-bagian dari sebuah tugas.

```csharp
public SplitPartCollection SplitParts { get; }
```

## Contoh

Menampilkan cara menampilkan bagian split tugas.

```csharp
var project = new Project(DataDir + "ViewSplitTasks.mpp");

// Akses tugas
var task = project.RootTask.Children.GetById(4);

// Tampilkan bagian split dari tugas
var collection = task.SplitParts;
foreach (var splitPart in collection)
{
    Console.WriteLine("Start: " + splitPart.Start + "\nFinish: " + splitPart.Finish + "\n");
}
```

### Lihat Juga

* class [SplitPartCollection](../../splitpartcollection/)
* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


