---
title: "Aspose::Tasks::Project::UpdateProjectWorkAsComplete metode"
linktitle: "UpdateProjectWorkAsComplete"
articleTitle: "UpdateProjectWorkAsComplete"
second_title: "Aspose.Tasks untuk C++"
description: "Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk seluruh proyek."
type: docs
weight: 2080
url: /id/cpp/aspose.tasks/project/updateprojectworkascomplete/
---

## UpdateProjectWorkAsComplete (1 of 2) {#updateprojectworkascomplete_1}

Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk seluruh proyek.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly)
```

| Parameter | Deskripsi |
| --- | --- |
| completeThrough | Tanggal untuk memperbarui pekerjaan sebagai selesai hingga. |
| setZeroOrHundredPercentCompleteOnly | Jika diatur ke true, hanya memperbarui tugas-tugas yang selesai 100% yang tanggal selesai-nya sebelum tanggal complete-through yang ditentukan. Jika tidak, menghitung nilai persentase selesai berdasarkan tanggal mulai terjadwal dan tanggal complete-through. |

---

## UpdateProjectWorkAsComplete (2 of 2) {#updateprojectworkascomplete_2}

Memperbarui semua pekerjaan sebagai selesai hingga tanggal yang ditentukan untuk daftar tugas yang ditentukan.

**Returns:** void Aspose::Tasks::

```cpp
UpdateProjectWorkAsComplete(System::DateTime completeThrough, bool setZeroOrHundredPercentCompleteOnly, const System::SharedPtr< System::Collections::Generic::List< System::SharedPtr< Task >>> & taskCollection)
```

| Parameter | Deskripsi |
| --- | --- |
| completeThrough | Tanggal untuk memperbarui pekerjaan sebagai selesai hingga. |
| setZeroOrHundredPercentCompleteOnly | Jika diatur ke true, hanya memperbarui tugas-tugas yang selesai 100% yang tanggal selesai-nya sebelum tanggal complete-through yang ditentukan. Jika tidak, menghitung nilai persentase selesai berdasarkan tanggal mulai terjadwal dan tanggal complete-through. |
| taskCollection | Daftar< Task > tugas untuk memperbarui pekerjaan. |

