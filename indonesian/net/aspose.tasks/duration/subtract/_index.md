---
title: "Duration.Subtract"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Duration. Mengurangi durasi yang ditentukan dari instance durasi ini"
type: docs
weight: 100
url: /id/net/aspose.tasks/duration/subtract/
---
## Subtract(Duration) {#subtract}

Mengurangi durasi yang ditentukan dari instance durasi ini.

```csharp
public Duration Subtract(Duration d)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| d | Duration | instance [`Duration`](../) yang ditentukan untuk dikurangi dari instance ini. |

### Nilai Kembali

Objek durasi baru yang mewakili nilai dari instance ini dikurangi nilai durasi yang ditentukan.

## Contoh

Menampilkan cara mengubah durasi tugas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);

// perbarui durasi tugas
var duration1 = task1.Get(Tsk.Duration);

// kurangi satu hari pada tugas 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// atur durasi baru ke tugas
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// dapatkan tugas lain
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// ubah durasi dengan menggunakan tipe unit waktu aktual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// atur durasi baru ke tugas
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)

---

## Subtract(double) {#subtract_1}

Mengurangi nilai double yang ditentukan dari instance durasi ini.

```csharp
public Duration Subtract(double val)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| val | Double | nilai Double yang ditentukan untuk dikurangi dari instance ini. |

### Nilai Kembali

Objek durasi baru yang mewakili nilai dari instance ini dikurangi nilai durasi yang ditentukan.

## Contoh

Menampilkan cara mengubah durasi tugas.

```csharp
var project = new Project(DataDir + "TaskDurations.mpp");

// dapatkan tugas
var task1 = project.RootTask.Children.GetById(1);

// perbarui durasi tugas
var duration1 = task1.Get(Tsk.Duration);

// kurangi satu hari pada tugas 1
duration1 = duration1.Subtract(project.GetDuration(1, TimeUnitType.Day));

// atur durasi baru ke tugas
task1.Set(Tsk.Duration, duration1);
Console.WriteLine("The duration of task 1: " + task1.Get(Tsk.Duration));

// dapatkan tugas lain
var task2 = project.RootTask.Children.GetById(2);
var duration2 = task2.Get(Tsk.Duration);

// ubah durasi dengan menggunakan tipe unit waktu aktual
Console.WriteLine("The time unit of duration: " + duration2.TimeUnit);
duration2 = duration2.Subtract(1d /* the time unit type of duration2 will be used */);

// atur durasi baru ke tugas
task2.Set(Tsk.Duration, duration2);
Console.WriteLine("The duration of task 2: " + task2.Get(Tsk.Duration));
```

### Lihat Juga

* struct [Duration](../)
* namespace [Aspose.Tasks](../../duration/)
* assembly [Aspose.Tasks](../../../)


