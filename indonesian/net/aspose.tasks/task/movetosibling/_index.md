---
title: "Task.MoveToSibling"
second_title: "Referensi API Aspose.Tasks untuk .NET"
description: "Metode Task. Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate setelah menggunakan metode ini. Itu akan menjadwalkan ulang semua tanggal mulai/selesai tugas proyek, mengatur tanggal awal/akhir, dan menghitung bidang tergantung seperti slack, kerja, dan biaya serta tingkat outline. Jika ParentProject.CalculationMode adalah Manual, metode ini akan menghitung hanya level outline dan nomor outline tugas secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis, mengatur tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, kerja, dan biaya, serta menghitung ulang ID dan level outline."
type: docs
weight: 1370
url: /id/net/aspose.tasks/task/movetosibling/
---
## MoveToSibling(Task) {#movetosibling}

Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwal ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwal ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

```csharp
public void MoveToSibling(Task beforeTask)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| beforeTask | Tugas | Tugas sebelum mana tugas saat ini akan disisipkan. |

## Contoh

Menampilkan cara memindahkan tugas di bawah induk yang sama.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Pindahkan tugas dengan id 5 sebelum tugas dengan id 3
var task = project.RootTask.Children.GetById(5);

var targetTask = project.RootTask.Children.First(t => t.Get(Tsk.Name) == "Task4");
task.MoveToSibling(targetTask);

// ATAU
// Pindahkan tugas ke akhir koleksi
// task.MoveToSibling(null);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)

---

## MoveToSibling(int) {#movetosibling_1}

Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas dengan Id yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwal ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwal ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

```csharp
public void MoveToSibling(int beforeTaskId)
```

| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| beforeTaskId | Int32 | Id ([`Id`](../../tsk/id/)) dari tugas sebelum mana tugas saat ini akan disisipkan. |

## Contoh

Menampilkan cara memindahkan tugas di bawah induk yang sama menggunakan Id tugas.

```csharp
var project = new Project(DataDir + "MoveTask.mpp");

// Pindahkan tugas dengan id 5 sebelum tugas dengan id 3
var task = project.RootTask.Children.GetById(5);

task.MoveToSibling(3);

// ATAU
// Pindahkan tugas ke akhir koleksi
// task.MoveToSibling(-1);
project.Save(OutDir + "MoveTaskUnderSameParent_out.mpp", SaveFileFormat.Mpp);
```

### Lihat Juga

* class [Task](../)
* namespace [Aspose.Tasks](../../task/)
* assembly [Aspose.Tasks](../../../)


