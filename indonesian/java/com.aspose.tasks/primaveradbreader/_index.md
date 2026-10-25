---
title: "PrimaveraDbReader"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pembaca untuk membaca Info Proyek dari DB Primavera"
type: docs
weight: 200
url: /id/java/com.aspose.tasks/primaveradbreader/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.PrimaveraBaseReader](../../com.aspose.tasks/primaverabasereader)
```
public final class PrimaveraDbReader extends PrimaveraBaseReader
```

Mewakili pembaca untuk membaca Info Proyek dari DB Primavera
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [PrimaveraDbReader(PrimaveraDbSettings dbSettings)](#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-) | Menginisialisasi instance baru dari kelas [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [loadProject(int projectUid)](#loadProject-int-) | Memuat proyek dengan pengidentifikasi unik yang ditentukan. |
### PrimaveraDbReader(PrimaveraDbSettings dbSettings) {#PrimaveraDbReader-com.aspose.tasks.PrimaveraDbSettings-}
```
public PrimaveraDbReader(PrimaveraDbSettings dbSettings)
```


Menginisialisasi instance baru dari kelas [PrimaveraXerReader](../../com.aspose.tasks/primaveraxerreader).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| dbSettings | [PrimaveraDbSettings](../../com.aspose.tasks/primaveradbsettings) | Pengaturan yang menentukan cara menghubungkan ke Primavera DB. |

### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Memuat proyek dengan pengidentifikasi unik yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| projectUid | int | Pengidentifikasi unik dari proyek yang akan dimuat. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier read from Primavera DB. Null if project doesn't exist.
