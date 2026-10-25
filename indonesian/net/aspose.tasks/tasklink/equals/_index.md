---
title: "TaskLink.Equals"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "TaskLink metode. Mengembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan"
type: docs
weight: 90
url: /id/net/aspose.tasks/tasklink/equals/
---
## Equals(TaskLink) {#equals}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public bool Equals(TaskLink other)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| other | TaskLink | Instance yang ditentukan dari kelas [`TaskLink`](../) untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified instance of the [`TaskLink`](../) class has the same predecessor and successor tasks as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan tautan tugas.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Kesetaraan tautan tugas didasarkan pada tugas pred dan succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Lihat Juga

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)

---

## Equals(object) {#equals_1}

Kembalikan nilai yang menunjukkan apakah instance ini sama dengan objek yang ditentukan.

```csharp
public override bool Equals(object obj)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| obj | Objek | Objek untuk dibandingkan dengan instance ini. |

### Nilai Kembali

**True** if the specified object is a TaskLink that has the same predecessor and successor as this instance; otherwise, **false**.

## Contoh

Menampilkan cara memeriksa kesetaraan tautan tugas.

```csharp
var project = new Project(DataDir + "GetPredecessorSuccessorTasks.mpp");

var link1 = project.TaskLinks[0];
var link2 = project.TaskLinks[1];

// Kesetaraan tautan tugas didasarkan pada tugas pred dan succ.
Console.Write("Link 1 Pred: " + link1.PredTask.ToString());
Console.Write("Link 1 Succ: " + link1.SuccTask.ToString());
Console.Write("Link 2 Pred: " + link2.PredTask.ToString());
Console.Write("Link 2 Succ: " + link2.SuccTask.ToString());
Console.Write("Are task links equal: " + link1.Equals(link2));
```

### Lihat Juga

* class [TaskLink](../)
* namespace [Aspose.Tasks](../../tasklink/)
* assembly [Aspose.Tasks](../../../)


