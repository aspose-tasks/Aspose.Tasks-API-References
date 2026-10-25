---
title: "Task.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan tugas yang ditentukan"
type: docs
weight: 1330
url: /id/net/aspose.tasks/task/equals/
---
## Equals(Task) {#equals}

Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan tugas yang ditentukan.

```csharp
public bool Equals(Task other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| lain | Tugas | Tugas yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika tugas yang ditentukan dan instance ini memiliki ID unik yang sama.

## Contoh

Menampilkan cara mengiterasi penugasan tugas.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // tampilkan penugasan tugas
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek yang ditentukan untuk dibandingkan dengan instance ini. |

### Nilai Kembali

mengembalikan true jika tugas yang ditentukan dan instance ini memiliki ID unik yang sama.

## Contoh

Menampilkan cara mengiterasi penugasan tugas.

```csharp
var project = new Project(DataDir + "BudgetWorkAndCost.mpp");

var collector = new ChildTasksCollector();
TaskUtils.Apply(project.RootTask, collector, 0);
foreach (var task in collector.Tasks)
{
    // tampilkan penugasan tugas
    foreach (var assignment in task.Assignments)
    {
        Console.WriteLine(assignment.ToString());
    }
}
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


