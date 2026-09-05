---
title: "ResourceLeveler"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Berisi metode penyeimbangan sumber daya."
type: docs
weight: 253
url: /id/java/com.aspose.tasks/resourceleveler/
---

**Inheritance:**
java.lang.Object
```
public class ResourceLeveler
```

Berisi metode penyeimbangan sumber daya.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ResourceLeveler()](#ResourceLeveler--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [clearLeveling(Project project)](#clearLeveling-com.aspose.tasks.Project-) | Menghapus setiap penundaan leveling yang sebelumnya ditambahkan ke proyek selama leveling sumber daya. |
| [clearLeveling(Iterable&lt;Task&gt; tasks)](#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--) | Menghapus setiap penundaan leveling yang sebelumnya ditambahkan ke tugas yang ditentukan selama leveling sumber daya. |
| [levelAll(Project project)](#levelAll-com.aspose.tasks.Project-) | Melakukan leveling tugas untuk semua sumber daya proyek menggunakan opsi leveling default. |
| [levelResources(Project project, LevelingOptions options)](#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-) | Melakukan leveling tugas untuk sumber daya yang ditentukan menggunakan opsi leveling yang ditentukan. |
### ResourceLeveler() {#ResourceLeveler--}
```
public ResourceLeveler()
```


### clearLeveling(Project project) {#clearLeveling-com.aspose.tasks.Project-}
```
public static void clearLeveling(Project project)
```


Menghapus setiap penundaan leveling yang sebelumnya ditambahkan ke proyek selama leveling sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyek untuk menghapus leveling. |

### clearLeveling(Iterable&lt;Task&gt; tasks) {#clearLeveling-java.lang.Iterable-com.aspose.tasks.Task--}
```
public static void clearLeveling(Iterable<Task> tasks)
```


Menghapus setiap penundaan leveling yang sebelumnya ditambahkan ke tugas yang ditentukan selama leveling sumber daya.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| tugas | java.lang.Iterable&lt;com.aspose.tasks.Task&gt; | Enumerable yang berisi tugas-tugas yang penundaan leveling-nya harus dihapus. |

### levelAll(Project project) {#levelAll-com.aspose.tasks.Project-}
```
public static LevelingResult levelAll(Project project)
```


Melakukan leveling tugas untuk semua sumber daya proyek menggunakan opsi leveling default.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyek untuk menerapkan leveling sumber daya. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
### levelResources(Project project, LevelingOptions options) {#levelResources-com.aspose.tasks.Project-com.aspose.tasks.LevelingOptions-}
```
public static LevelingResult levelResources(Project project, LevelingOptions options)
```


Melakukan leveling tugas untuk sumber daya yang ditentukan menggunakan opsi leveling yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| project | [Project](../../com.aspose.tasks/project) | Proyek untuk menerapkan leveling sumber daya. |
| options | [LevelingOptions](../../com.aspose.tasks/levelingoptions) | Opsi yang menentukan cara melakukan leveling sumber daya. |

**Returns:**
[LevelingResult](../../com.aspose.tasks/levelingresult) - Object containing results of resource leveling.
