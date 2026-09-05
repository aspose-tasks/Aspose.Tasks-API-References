---
title: "TaskUtils"
second_title: "Referensi API Aspose.Tasks for Java"
description: "Kelas pembantu yang menyediakan operasi berguna dengan tugas."
type: docs
weight: 307
url: /id/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Kelas pembantu yang menyediakan operasi berguna dengan tugas.
## Konstruktor

| Konstruktor | Deskripsi |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Metode

| Metode | Deskripsi |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Menerapkan algoritma yang ditentukan ke setiap tugas dalam sebuah pohon. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Membangun pohon baru tugas yang memenuhi kondisi. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Menemukan tugas yang memenuhi kondisi dalam sebuah pohon tugas. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Menghitung secara rekursif jumlah anak tugas melalui semua level. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Menerapkan algoritma yang ditentukan ke setiap tugas dalam sebuah pohon.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Akar pohon |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Algoritma yang diterapkan. |
| tingkat | int | Tingkat dari tugas akar. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Membangun pohon baru tugas yang memenuhi kondisi.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Akar pohon. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Kondisi yang diterapkan. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Menemukan tugas yang memenuhi kondisi dalam sebuah pohon tugas.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Akar pohon. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Kondisi yang diterapkan. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Menghitung secara rekursif jumlah anak tugas melalui semua level.

**Parameters:**
| Parameter | Tipe | Deskripsi |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Tugas yang anak-anaknya dihitung. |

**Returns:**
int - Jumlah anak.
