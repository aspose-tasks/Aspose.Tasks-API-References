---
title: "SimpleSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bu, bir projeyi belirli bir formata kaydederken kullanıcının temel seçenekleri belirtmesine izin veren soyut bir temel sınıftır."
type: docs
weight: 277
url: /tr/java/com.aspose.tasks/simplesaveoptions/
---

**Inheritance:**
java.lang.Object
```
public abstract class SimpleSaveOptions
```

Bu, bir projeyi belirli bir formata kaydederken kullanıcının temel seçenekleri belirtmesine izin veren soyut bir temel sınıftır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [SimpleSaveOptions()](#SimpleSaveOptions--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getSaveFormat()](#getSaveFormat--) | Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği formatı alır. |
| [getTasksComparer()](#getTasksComparer--) | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır. |
| [getTasksFilter()](#getTasksFilter--) | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında render edilen görevleri filtrelemek için kullanılan koşulu alır. |
| [setTasksComparer(Comparator&lt;Task&gt; value)](#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--) | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı ayarlar. |
| [setTasksFilter(ICondition&lt;Task&gt; value)](#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--) | Gantt, Görev Sayfası ve Görev Kullanımı şemalarında render edilen görevleri filtrelemek için kullanılan koşulu ayarlar. |
### SimpleSaveOptions() {#SimpleSaveOptions--}
```
public SimpleSaveOptions()
```


### getSaveFormat() {#getSaveFormat--}
```
public final int getSaveFormat()
```


Bu kaydetme seçenekleri nesnesi kullanılırsa belgenin kaydedileceği formatı alır.

**Returns:**
int - belgenin kaydedileceği [SaveFileFormat](../../com.aspose.tasks/savefileformat).
### getTasksComparer() {#getTasksComparer--}
```
public final Comparator<Task> getTasksComparer()
```


Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı alır.

**Returns:**
java.util.Comparator&lt;com.aspose.tasks.Task&gt; - Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcı.
### getTasksFilter() {#getTasksFilter--}
```
public final ICondition<Task> getTasksFilter()
```


Gantt, Görev Sayfası ve Görev Kullanımı şemalarında render edilen görevleri filtrelemek için kullanılan koşulu alır.

--------------------

Değer belirtilmezse, görünmeyen görevleri (yani daraltılmış görevlerin alt görevlerini) kaldıran varsayılan filtre kullanılır.

**Returns:**
[ICondition](../../com.aspose.tasks/icondition) - the condition which is used to filter tasks rendered on Gantt, Task Sheet and Task Usage charts.
### setTasksComparer(Comparator&lt;Task&gt; value) {#setTasksComparer-java.util.Comparator-com.aspose.tasks.Task--}
```
public final void setTasksComparer(Comparator<Task> value)
```


Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcıyı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Comparator&lt;com.aspose.tasks.Task&gt; | Gantt şeması ve Görev Sayfası şemasındaki görevleri sıralamak için karşılaştırıcı. |

### setTasksFilter(ICondition&lt;Task&gt; value) {#setTasksFilter-com.aspose.tasks.ICondition-com.aspose.tasks.Task--}
```
public final void setTasksFilter(ICondition<Task> value)
```


Gantt, Görev Sayfası ve Görev Kullanımı şemalarında render edilen görevleri filtrelemek için kullanılan koşulu ayarlar.

--------------------

Değer belirtilmezse, görünmeyen görevleri (yani daraltılmış görevlerin alt görevlerini) kaldıran varsayılan filtre kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | com.aspose.tasks.ICondition&lt;com.aspose.tasks.Task&gt; | Gantt, Görev Sayfası ve Görev Kullanımı grafiklerinde oluşturulan görevleri filtrelemek için kullanılan koşul. |

