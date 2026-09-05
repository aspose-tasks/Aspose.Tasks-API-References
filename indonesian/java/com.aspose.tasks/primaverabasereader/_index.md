---
title: "PrimaveraBaseReader"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili pembaca dasar yang dapat digunakan untuk membaca UID Proyek dari file Primavera XER atau XML multi proyek."
type: docs
weight: 196
url: /id/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Mewakili pembaca dasar yang dapat digunakan untuk membaca UID Proyek dari file Primavera XER atau XML multi proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Kembalikan daftar objek info singkat proyek. |
| [getProjectUids()](#getProjectUids--) | Kembalikan daftar pengidentifikasi unik proyek-proyek. |
| [loadProject(int projectUid)](#loadProject-int-) | Memuat proyek dengan pengidentifikasi unik yang ditentukan. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Kembalikan daftar objek info singkat proyek.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - daftar objek info singkat proyek.
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Kembalikan daftar pengidentifikasi unik proyek-proyek.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - Daftar pengidentifikasi unik proyek-proyek.
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
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
