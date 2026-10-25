---
title: "RemoveTask"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Menghapus tugas yang ditentukan dari pohon tugas."
type: docs
weight: 246
url: /id/java/com.aspose.tasks/removetask/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.tasks.ITreeAlgorithm
```
public class RemoveTask implements ITreeAlgorithm<Task>
```

Menghapus tugas yang ditentukan dari pohon tugas.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [RemoveTask(Task task)](#RemoveTask-com.aspose.tasks.Task-) | Menginisialisasi instance baru dari kelas [RemoveTask](../../com.aspose.tasks/removetask). |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Tidak melakukan apa‑apa. |
| [postAlg(Task el, int level)](#postAlg-com.aspose.tasks.Task-int-) | Tidak melakukan apa‑apa. |
| [preAlg(Task el, int level)](#preAlg-com.aspose.tasks.Task-int-) | Menghapus tugas dari tugas induk yang ditentukan. |
### RemoveTask(Task task) {#RemoveTask-com.aspose.tasks.Task-}
```
public RemoveTask(Task task)
```


Menginisialisasi instance baru dari kelas [RemoveTask](../../com.aspose.tasks/removetask).

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tugas yang akan dihapus. |

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public final void alg(Task el, int level)
```


Tidak melakukan apa‑apa.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objek untuk diproses. |
| tingkat | int | Level node pohon. |

### postAlg(Task el, int level) {#postAlg-com.aspose.tasks.Task-int-}
```
public final void postAlg(Task el, int level)
```


Tidak melakukan apa‑apa.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Objek untuk diproses. |
| tingkat | int | Level node pohon. |

### preAlg(Task el, int level) {#preAlg-com.aspose.tasks.Task-int-}
```
public final void preAlg(Task el, int level)
```


Menghapus tugas dari tugas induk yang ditentukan.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | Tugas induk. |
| tingkat | int | Level node pohon. |

