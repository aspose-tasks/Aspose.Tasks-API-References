---
title: "ChildTasksCollector"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Tüm alt görevleri toplar."
type: docs
weight: 49
url: /tr/java/com.aspose.tasks/childtaskscollector/
---

**Inheritance:**
java.lang.Object, com.aspose.tasks.TreeAlgorithmBase
```
public class ChildTasksCollector extends TreeAlgorithmBase<Task>
```

Tüm alt görevleri toplar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ChildTasksCollector()](#ChildTasksCollector--) | Yeni bir [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [alg(Task el, int level)](#alg-com.aspose.tasks.Task-int-) | Belirtilen nesneyi işler. |
| [getTasks()](#getTasks--) | Toplanan alt nesnelerin (görevlerin) bir listesini alır. |
### ChildTasksCollector() {#ChildTasksCollector--}
```
public ChildTasksCollector()
```


Yeni bir [ChildTasksCollector](../../com.aspose.tasks/childtaskscollector) sınıfının örneğini başlatır.

### alg(Task el, int level) {#alg-com.aspose.tasks.Task-int-}
```
public void alg(Task el, int level)
```


Belirtilen nesneyi işler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| el | [Task](../../com.aspose.tasks/task) | İşlenecek nesne. |
| seviye | int | Ağaç düğüm seviyesi. |

### getTasks() {#getTasks--}
```
public final List<Task> getTasks()
```


Toplanan alt nesnelerin (görevlerin) bir listesini alır.

**Returns:**
java.util.List<com.aspose.tasks.Task> - toplanan alt nesnelerin (görevlerin) bir listesi.
