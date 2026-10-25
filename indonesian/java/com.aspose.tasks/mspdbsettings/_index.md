---
title: "MspDbSettings"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan mengatur opsi yang diperlukan untuk membaca data proyek dari basis data MS Project Server."
type: docs
weight: 161
url: /id/java/com.aspose.tasks/mspdbsettings/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.DbSettings](../../com.aspose.tasks/dbsettings)
```
public class MspDbSettings extends DbSettings
```

Memungkinkan mengatur opsi yang diperlukan untuk membaca data proyek dari basis data MS Project Server.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [MspDbSettings(String connectionString, UUID projectGuid)](#MspDbSettings-java.lang.String-java.util.UUID-) | Menginisialisasi instance baru dari kelas [MspDbSettings](../../com.aspose.tasks/mspdbsettings). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getProjectGuid()](#getProjectGuid--) | Mendapatkan guid proyek yang akan dibaca. |
| [getSchema()](#getSchema--) | Mendapatkan skema MS Project Server. |
| [setSchema(String value)](#setSchema-java.lang.String-) | Mengatur skema MS Project Server. |
### MspDbSettings(String connectionString, UUID projectGuid) {#MspDbSettings-java.lang.String-java.util.UUID-}
```
public MspDbSettings(String connectionString, UUID projectGuid)
```


Menginisialisasi instance baru dari kelas [MspDbSettings](../../com.aspose.tasks/mspdbsettings).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| connectionString | java.lang.String | string koneksi yang ditentukan. |
| projectGuid | java.util.UUID | guid yang ditentukan dari proyek yang akan dibaca. |

### getProjectGuid() {#getProjectGuid--}
```
public final UUID getProjectGuid()
```


Mendapatkan guid proyek yang akan dibaca.

**Returns:**
java.util.UUID - guid proyek yang akan dibaca.
### getSchema() {#getSchema--}
```
public final String getSchema()
```


Mendapatkan skema MS Project Server. Nilai default adalah "pub".

**Returns:**
java.lang.String - skema MS Project Server.
### setSchema(String value) {#setSchema-java.lang.String-}
```
public final void setSchema(String value)
```


Mengatur skema MS Project Server. Nilai default adalah "pub".

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | skema MS Project Server. |

