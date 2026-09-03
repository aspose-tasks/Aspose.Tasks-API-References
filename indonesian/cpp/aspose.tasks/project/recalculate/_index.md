---
title: "Aspose::Tasks::Project::Recalculate metode"
linktitle: "Recalculate"
articleTitle: "Recalculate"
second_title: "Aspose.Tasks untuk C++"
description: "Menjadwalkan ulang semua ids tugas proyek, level outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya."
type: docs
weight: 1130
url: /id/cpp/aspose.tasks/project/recalculate/
---

## Recalculate (1 of 2) {#recalculate_1}

Menjadwalkan ulang semua ids tugas proyek, level outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate()
```

---

## Recalculate (2 of 2) {#recalculate_2}

Menjadwalkan ulang semua ID tugas proyek, tingkat outline, tanggal mulai/selesai, mengatur tanggal awal/akhir, menghitung slack, bidang kerja dan biaya dengan validasi opsional.

**Returns:** void Aspose::Tasks::

```cpp
Recalculate(bool validate)
```

| Parameter | Deskripsi |
| --- | --- |
| validasi | Jika true, validasi perhitungan ulang akan dilakukan. Data apa yang divalidasi: Saat ini hanya validasi dasar rentang tanggal tugas dan tautan tugas yang diimplementasikan. Rentang tanggal tugas (mis. ActualStart - ActualFinish, EarlyStart - EarlyFinish, dll.) serta tanggal Task Links akan diperiksa terhadap kriteria tanggal bahwa tanggal mulai kurang atau sama dengan tanggal selesai. Jika salah satu kondisi yang dijelaskan di atas gagal, maka RecalculationValidationException akan dilempar. |

