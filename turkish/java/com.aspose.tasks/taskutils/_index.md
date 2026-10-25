---
title: "TaskUtils"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Görevlerle ilgili faydalı işlemler sağlayan yardımcı sınıf."
type: docs
weight: 307
url: /tr/java/com.aspose.tasks/taskutils/
---

**Inheritance:**
java.lang.Object
```
public class TaskUtils
```

Görevlerle ilgili faydalı işlemler sağlayan yardımcı sınıf.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TaskUtils()](#TaskUtils--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level)](#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-) | Belirtilen algoritmayı bir ağacın her görevine uygular. |
| [filter(Task root, ICondition&lt;Task&gt; cond)](#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Koşulu sağlayan görevlerin yeni bir ağacını oluşturur. |
| [find(Task root, ICondition&lt;Task&gt; cond)](#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Görev ağacında koşulu sağlayan bir görevi bulur. |
| [taskChildrenCount(Task task)](#taskChildrenCount-com.aspose.tasks.Task-) | Tüm seviyelerde görevlerin alt görev sayısını özyinelemeli olarak hesaplar. |
### TaskUtils() {#TaskUtils--}
```
public TaskUtils()
```


### apply(Task root, ITreeAlgorithm&lt;Task&gt; alg, int level) {#apply-com.aspose.tasks.Task-com.aspose.tasks.ITreeAlgorithm-com.aspose.tasks.Task--int-}
```
public static void apply(Task root, ITreeAlgorithm<Task> alg, int level)
```


Belirtilen algoritmayı bir ağacın her görevine uygular.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ağacın kökü |
| alg | com.aspose.tasks.ITreeAlgorithm&lt;com.aspose.tasks.Task&gt; | Uygulanan algoritma. |
| seviye | int | Kök görevin seviyesi. |

### filter(Task root, ICondition&lt;Task&gt; cond) {#filter-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task filter(Task root, ICondition<Task> cond)
```


Koşulu sağlayan görevlerin yeni bir ağacını oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ağacın kökü. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Uygulanan koşul. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Root of a new tree.
### find(Task root, ICondition&lt;Task&gt; cond) {#find-com.aspose.tasks.Task-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public static Task find(Task root, ICondition<Task> cond)
```


Görev ağacında koşulu sağlayan bir görevi bulur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| root | [Task](../../com.aspose.tasks/task) | Ağacın kökü. |
| cond | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Uygulanan koşul. |

**Returns:**
[Task](../../com.aspose.tasks/task) - Task if task was found, otherwise null.
### taskChildrenCount(Task task) {#taskChildrenCount-com.aspose.tasks.Task-}
```
public static int taskChildrenCount(Task task)
```


Tüm seviyelerde görevlerin alt görev sayısını özyinelemeli olarak hesaplar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| task | [Task](../../com.aspose.tasks/task) | Alt görevleri hesaplanan görev. |

**Returns:**
int - Alt görev sayısı.
