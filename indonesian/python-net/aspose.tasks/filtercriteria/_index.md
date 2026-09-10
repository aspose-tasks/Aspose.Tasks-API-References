---
title: "FilterCriteria"
second_title: "Referensi API Aspose.Tasks untuk Python via .NET"
description: 
type: docs
weight: 350
url: /id/python-net/aspose.tasks/filtercriteria/
---

## FilterCriteria class

Mendefinisikan kriteria yang harus dipenuhi oleh tugas atau sumber daya untuk ditampilkan dalam tampilan MSP.

Tipe FilterCriteria menampilkan anggota-anggota berikut:
## Konstruktor
| Nama | Deskripsi |
| :- | :- |
| FilterCriteria() | Menginisialisasi sebuah instance baru dari kelas FilterCriteria |
## Properti
| Nama | Deskripsi |
| :- | :- |
| operasi | Mendapatkan atau mengatur kriteria yang ditetapkan dengan FieldName, Test, dan Value yang berhubungan dengan kriteria lain dalam filter. |
| field | Mendapatkan atau mengatur sebuah [field](/tasks/python-net/aspose.tasks/filtercriteria/) untuk diubah. |
| test | Mendapatkan atau mengatur tipe perbandingan yang dibuat antara FieldName dan Value yang berfungsi sebagai kriteria seleksi untuk filter.<br/>            [FilterComparisonType](/tasks/python-net/aspose.tasks/filtercomparisontype/) |
| values | Mendapatkan nilai objek untuk dibandingkan dengan nilai bidang yang ditentukan dengan FieldName. |
| criteria_rows | Mendapatkan daftar baris [FilterCriteria](/tasks/python-net/aspose.tasks/filtercriteria/) anak.<br/>            Jika filter berisi lebih dari satu baris kriteria, maka efek dari operator And adalah bahwa kriteria untuk kedua baris harus dipenuhi agar tugas atau sumber daya ditampilkan sebagai hasil dari filter ini.<br/>            Efek dari operator Or adalah bahwa kriteria untuk salah satu baris harus dipenuhi. |
## Methods
| Nama | Deskripsi |
| :- | :- |
| is_field_value() | Mendapatkan apakah nilai sisi kanan FilterCriteria adalah referensi bidang, bukan nilai konstan. |
| set_value_field(value) | Mengatur bidang yang nilainya akan dibandingkan dengan nilai bidang yang ditentukan oleh FieldName. |

### Lihat Juga

* namespace [aspose.tasks](/tasks/python-net/aspose.tasks/)
* assembly [Aspose.Tasks](/tasks/python-net/)

