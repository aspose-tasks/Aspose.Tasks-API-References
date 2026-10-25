---
title: "Aspose::Tasks::Project::GetPageCount metode"
linktitle: "GetPageCount"
articleTitle: "GetPageCount"
second_title: "Aspose.Tasks untuk C++"
description: "Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale default (Hari)."
type: docs
weight: 1090
url: /id/cpp/aspose.tasks/project/getpagecount/
---

## GetPageCount (1 of 7) {#getpagecount_1}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale default (Hari).

**Returns:** Page count to be rendered.

```cpp
GetPageCount()
```

---

## GetPageCount (2 of 7) {#getpagecount_2}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan SaveOptions yang diberikan.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(const System::SharedPtr< Saving::SaveOptions > & saveOptions)
```

| Parameter | Deskripsi |
| --- | --- |
| saveOptions | Opsi penyimpanan untuk mendapatkan jumlah halaman. |

---

## GetPageCount (3 of 7) {#getpagecount_3}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale dan PageSize yang diberikan.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale)
```

| Parameter | Deskripsi |
| --- | --- |
| pageSize | Ukuran untuk mendapatkan jumlah halaman. |
| scale | Skala untuk mendapatkan jumlah halaman. |

---

## GetPageCount (4 of 7) {#getpagecount_4}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale, PresentationFormat, dan rentang tanggal yang diberikan.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PageSize pageSize, Visualization::Timescale scale, System::DateTime startDate, System::DateTime endDate)
```

| Parameter | Deskripsi |
| --- | --- |
| pageSize | Ukuran untuk mendapatkan jumlah halaman. |
| scale | Skala untuk mendapatkan jumlah halaman. |
| startDate | Tanggal mulai untuk mendapatkan jumlah halaman. |
| endDate | Tanggal akhir untuk mendapatkan jumlah halaman. |

---

## GetPageCount (5 of 7) {#getpagecount_5}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale default (Hari) dan PresentationFormat yang diberikan

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format)
```

| Parameter | Deskripsi |
| --- | --- |
| format | Format untuk mendapatkan jumlah halaman. |

---

## GetPageCount (6 of 7) {#getpagecount_6}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale dan PresentationFormat yang diberikan.

**Returns:** a page count to be rendered.

```cpp
GetPageCount(Visualization::PresentationFormat format, Visualization::Timescale scale)
```

| Parameter | Deskripsi |
| --- | --- |
| format | Format untuk mendapatkan jumlah halaman. |
| scale | Skala untuk mendapatkan jumlah halaman. |

---

## GetPageCount (7 of 7) {#getpagecount_7}

Mengembalikan jumlah halaman untuk proyek yang akan dirender menggunakan Timescale yang diberikan.

**Returns:** Page count to be rendered.

```cpp
GetPageCount(Visualization::Timescale scale)
```

| Parameter | Deskripsi |
| --- | --- |
| scale | Skala untuk mendapatkan jumlah halaman. |

