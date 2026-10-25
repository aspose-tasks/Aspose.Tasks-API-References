---
title: "ChildTasksCollector"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Mengumpulkan semua tugas anak."
type: docs
weight: 49
url: /id/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Mengumpulkan semua tugas anak.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Menginisialisasi sebuah instance baru dari kelas [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Memproses objek yang ditentukan. |
| [getTasks()](#getTasks--) | Mendapatkan daftar objek anak yang dikumpulkan (tugas). |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Menginisialisasi sebuah instance baru dari kelas [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector).

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Memproses objek yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objek untuk diproses. |
| tingkat | int | Level node pohon. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Mendapatkan daftar objek anak yang dikumpulkan (tugas).

**Returns:**
java.util.List<com.aspose.tasks.Task> - sebuah daftar objek anak yang dikumpulkan (tugas).
