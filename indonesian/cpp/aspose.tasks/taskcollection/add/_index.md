---
title: "Aspose::Tasks::TaskCollection::Add metode"
linktitle: "Add"
articleTitle: "Add"
second_title: "Aspose.Tasks untuk C++"
description: "Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir."
type: docs
weight: 10
url: /id/cpp/aspose.tasks/taskcollection/add/
---

## Add (1 of 5) {#add_1}

Menambahkan tugas baru ke koleksi tugas proyek pada tingkat outline yang sama dengan tugas terakhir.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add()
```

---

## Add (2 of 5) {#add_2}

Menyisipkan tugas baru sebelum tugas dengan id yang ditentukan dan pada tingkat outline yang sama.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::SharedPtr< RecurringTaskParameters > & parameters)
```

| Parameter | Deskripsi |
| --- | --- |
| parameter | Parameter yang ditentukan untuk pembuatan tugas berulang. |

---

## Add (3 of 5) {#add_3}

Tambahkan tugas yang ditentukan ke instance kelas TaskCollection. Jika ParentProject.CalculationMode adalah None, pengguna harus memanggil Project.Recalculate() setelah menggunakan metode ini (Ini akan menjadwalkan ulang semua tugas proyek (tanggal mulai/selesai, mengatur tanggal awal/akhir) dan menghitung bidang yang bergantung seperti slack, bidang kerja dan biaya, id, serta tingkat outline). Jika ParentProject.CalculationMode adalah Manual, metode ini akan menghitung hanya id tugas, tingkat outline, dan nomor outline secara otomatis. Jika ParentProject.CalculationMode adalah Automatic, metode ini menjadwalkan ulang semua tugas proyek secara otomatis (tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya, menghitung ulang id dan tingkat outline).

**Returns:** void Aspose::Tasks::

```cpp
Add(const System::SharedPtr< Task > & item)
```

| Parameter | Deskripsi |
| --- | --- |
| item | tugas yang ditentukan yang harus ditambahkan ke koleksi tugas ini. |

---

## Add (4 of 5) {#add_4}

Menambahkan tugas baru ke koleksi tugas anak.

**Returns:** returns the newly added instance of the Task class.

```cpp
Add(const System::String & taskName)
```

| Parameter | Deskripsi |
| --- | --- |
| taskName | nama tugas yang ditentukan. |

---

## Add (5 of 5) {#add_5}

Menambahkan tugas berulang baru ke koleksi tugas anak.

**Returns:** returns a task which was inserted before a task with the specified id.

```cpp
Add(const System::String & taskName, int32_t beforeTaskId)
```

| Parameter | Deskripsi |
| --- | --- |
| taskName | nama tugas yang ditentukan. |
| beforeTaskId | ID yang ditentukan dari sebuah tugas sebelum mana tugas baru akan disisipkan. |

