---
title: "Aspose::Tasks::Task::MoveToSibling metode"
linktitle: "MoveToSibling"
articleTitle: "MoveToSibling"
second_title: "Aspose.Tasks untuk C++"
description: "Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas yang ditentukan."
type: docs
weight: 1370
url: /id/cpp/aspose.tasks/task/movetosibling/
---

## MoveToSibling (1 of 2) {#movetosibling_1}

Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwal ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini hanya akan menghitung id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwal ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(const System::SharedPtr< Task > & beforeTask)
```

| Parameter | Deskripsi |
| --- | --- |
| beforeTask | Tugas sebelum mana tugas saat ini akan disisipkan. |

---

## MoveToSibling (2 of 2) {#movetosibling_2}

Memindahkan tugas saat ini pada Tingkat Outline yang sama sebelum tugas dengan Id yang ditentukan. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini akan menghitung hanya id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

**Returns:** void Aspose::Tasks::

```cpp
MoveToSibling(int32_t beforeTaskId)
```

| Parameter | Deskripsi |
| --- | --- |
| beforeTaskId | Id ( Tsk::Id ) dari tugas sebelum mana tugas saat ini akan disisipkan. |

