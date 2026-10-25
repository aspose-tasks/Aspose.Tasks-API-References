---
title: "PrimaveraBaseReader"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Çoklu proje Primavera XER veya XML dosyalarından Proje UID'lerini okumak için kullanılabilen temel bir okuyucuyu temsil eder."
type: docs
weight: 196
url: /tr/java/com.aspose.tasks/primaverabasereader/
---

**Inheritance:**
java.lang.Object
```
public abstract class PrimaveraBaseReader
```

Çoklu proje Primavera XER veya XML dosyalarından Proje UID'lerini okumak için kullanılabilen temel bir okuyucuyu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getProjectInfos()](#getProjectInfos--) | Projenin kısa bilgi nesnelerinin bir listesini döndürür. |
| [getProjectUids()](#getProjectUids--) | Projelerin benzersiz tanımlayıcılarının bir listesini döndürür. |
| [loadProject(int projectUid)](#loadProject-int-) | Belirtilen benzersiz tanımlayıcı ile projeyi yükler. |
### getProjectInfos() {#getProjectInfos--}
```
public final List<PrimaveraProjectInfo> getProjectInfos()
```


Projenin kısa bilgi nesnelerinin bir listesini döndürür.

**Returns:**
java.util.List&lt;com.aspose.tasks.PrimaveraProjectInfo&gt; - projenin kısa bilgi nesnelerinin bir listesi
### getProjectUids() {#getProjectUids--}
```
public final List<Integer> getProjectUids()
```


Projelerin benzersiz tanımlayıcılarının bir listesini döndürür.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - projelerin benzersiz tanımlayıcılarının listesi.
### loadProject(int projectUid) {#loadProject-int-}
```
public Project loadProject(int projectUid)
```


Belirtilen benzersiz tanımlayıcı ile projeyi yükler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| projectUid | int | Yüklenmekte olan projenin benzersiz tanımlayıcısı. |

**Returns:**
[Project](../../com.aspose.tasks/project) - Project with specified unique identifier from the specified multi project file. Null if project doesn't exist.
