---
title: "VbaModule"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mewakili modul VBA."
type: docs
weight: 334
url: /id/java/com.aspose.tasks/vbamodule/
---

**Inheritance:**
java.lang.Object
```
public final class VbaModule
```

Mewakili modul VBA.
## Metode

| Metode | Deskripsi |
| --- | --- |
| [createClassModule(String name)](#createClassModule-java.lang.String-) | Membuat sebuah instance dari [VbaModule](../../com.aspose/tasks/vbamodule) dengan tipe VbaModuleType.ClassModule. |
| [createProceduralModule(String name)](#createProceduralModule-java.lang.String-) | Membuat sebuah instance dari [VbaModule](../../com.aspose/tasks/vbamodule) dengan tipe VbaModuleType.ProceduralModule. |
| [getAttributes()](#getAttributes--) | Mendapatkan koleksi atribut modul. |
| [getName()](#getName--) | Mendapatkan nama modul VBA. |
| [getSourceCode()](#getSourceCode--) | Mendapatkan kode sumber modul VBA. |
| [getType()](#getType--) | Mendapatkan tipe modul. |
| [setName(String value)](#setName-java.lang.String-) | Nama modul VBA. |
| [setSourceCode(String value)](#setSourceCode-java.lang.String-) | Mengatur kode sumber modul VBA. |
### createClassModule(String name) {#createClassModule-java.lang.String-}
```
public static VbaModule createClassModule(String name)
```


Membuat sebuah instance dari [VbaModule](../../com.aspose/tasks/vbamodule) dengan tipe VbaModuleType.ClassModule.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### createProceduralModule(String name) {#createProceduralModule-java.lang.String-}
```
public static VbaModule createProceduralModule(String name)
```


Membuat sebuah instance dari [VbaModule](../../com.aspose/tasks/vbamodule) dengan tipe VbaModuleType.ProceduralModule.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[VbaModule](../../com.aspose.tasks/vbamodule)
### getAttributes() {#getAttributes--}
```
public final VbaModuleAttributeCollection getAttributes()
```


Mendapatkan koleksi atribut modul.

**Returns:**
[VbaModuleAttributeCollection](../../com.aspose.tasks/vbamoduleattributecollection) - a collection of the module's attributes.
### getName() {#getName--}
```
public final String getName()
```


Mendapatkan nama modul VBA.

**Returns:**
java.lang.String - nama modul VBA.
### getSourceCode() {#getSourceCode--}
```
public final String getSourceCode()
```


Mendapatkan kode sumber modul VBA.

**Returns:**
java.lang.String - kode sumber modul VBA.
### getType() {#getType--}
```
public final int getType()
```


Mendapatkan tipe modul.

**Returns:**
int - tipe modul.
### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Nama modul VBA.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | nama modul VBA. |

### setSourceCode(String value) {#setSourceCode-java.lang.String-}
```
public final void setSourceCode(String value)
```


Mengatur kode sumber modul VBA.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| nilai | java.lang.String | kode sumber modul VBA. |

