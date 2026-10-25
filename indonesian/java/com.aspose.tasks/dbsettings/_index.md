---
title: "DbSettings"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Memungkinkan untuk menentukan pengaturan untuk membaca dari basis data proyek."
type: docs
weight: 75
url: /id/java/com.aspose.tasks/dbsettings/
---

**Inheritance:**
java.lang.Object
```
public abstract class DbSettings
```

Memungkinkan untuk menentukan pengaturan untuk membaca dari basis data proyek.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [getConnectionString()](#getConnectionString--) | Mendapatkan string koneksi. |
| [getDriverClassName()](#getDriverClassName--) | Mengembalikan nama kelas driver JDBC. |
| [setConnectionString(String value)](#setConnectionString-java.lang.String-) | Mengatur string koneksi. |
| [setDriverClassName(String value)](#setDriverClassName-java.lang.String-) | Mengatur nama kelas driver JDBC. |
### getConnectionString() {#getConnectionString--}
```
public final String getConnectionString()
```


Mendapatkan string koneksi.

**Returns:**
java.lang.String - string koneksi.
### getDriverClassName() {#getDriverClassName--}
```
public final String getDriverClassName()
```


Mengembalikan nama kelas driver JDBC. Nama kelas driver default adalah "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Returns:**
java.lang.String - string kelas driver.
### setConnectionString(String value) {#setConnectionString-java.lang.String-}
```
public final void setConnectionString(String value)
```


Mengatur string koneksi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | string koneksi. |

### setDriverClassName(String value) {#setDriverClassName-java.lang.String-}
```
public final void setDriverClassName(String value)
```


Mengatur nama kelas driver JDBC. Nama kelas driver default adalah "com.microsoft.jdbc.sqlserver.SQLServerDriver"

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama kelas driver JDBC. |

