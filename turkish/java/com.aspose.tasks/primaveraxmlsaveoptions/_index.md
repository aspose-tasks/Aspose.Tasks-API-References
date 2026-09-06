---
title: "PrimaveraXmlSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeyi Primavera xml formatına kaydederken ek seçeneklerin belirtilmesine izin verir."
type: docs
weight: 212
url: /tr/java/com.aspose.tasks/primaveraxmlsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraXmlSaveOptions extends SimpleSaveOptions
```

Projeyi Primavera xml formatına kaydederken ek seçeneklerin belirtilmesine izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PrimaveraXmlSaveOptions()](#PrimaveraXmlSaveOptions--) | Yeni bir [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) sınıf örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getSaveRootTask()](#getSaveRootTask--) | Kök görevi kaydedip kaydetmeyeceğini gösteren bir değeri alır. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır. |
| [setSaveRootTask(boolean value)](#setSaveRootTask-boolean-) | Kök görevi kaydedip kaydetmeyeceğini gösteren bir değeri ayarlar. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri ayarlar. |
### PrimaveraXmlSaveOptions() {#PrimaveraXmlSaveOptions--}
```
public PrimaveraXmlSaveOptions()
```


Yeni bir [PrimaveraXmlSaveOptions](../../com.aspose.tasks/primaveraxmlsaveoptions) sınıf örneği başlatır.

### getSaveRootTask() {#getSaveRootTask--}
```
public final boolean getSaveRootTask()
```


Kök görevi kaydedip kaydetmeyeceğini gösteren bir değeri alır.

**Returns:**
boolean - bir kök görevi kaydedip kaydetmeyeceğini belirten bir değer.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır.

Primavera yazılımı, kaynakların özet (WBS) görevlerine atanmasını desteklemez. Bu nedenle, bu tür atamaların dışa aktarılması Primavera modeline göre geçersiz bir dosyaya yol açabilir. Eğer true ise, özet görevlere atamalar dışa aktarım sırasında atlanır. Eğer false (varsayılan değer) ise, dışa aktarım sırasında bir özet göreve atama bulunursa bir istisna fırlatılacaktır.

**Returns:**
boolean - kaynakların özet görevlere atanmasının dışa aktarım sırasında atlanıp atlanmayacağını belirten bir değer.
### setSaveRootTask(boolean value) {#setSaveRootTask-boolean-}
```
public final void setSaveRootTask(boolean value)
```


Kök görevi kaydedip kaydetmeyeceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir kök görevi kaydedip kaydetmeyeceğini belirten bir değer. |

### setSkipSummaryAssignments(boolean value) {#setSkipSummaryAssignments-boolean-}
```
public final void setSkipSummaryAssignments(boolean value)
```


Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri ayarlar.

Primavera yazılımı, kaynakların özet (WBS) görevlerine atanmasını desteklemez. Bu nedenle, bu tür atamaların dışa aktarılması Primavera modeline göre geçersiz bir dosyaya yol açabilir. Eğer true ise, özet görevlere atamalar dışa aktarım sırasında atlanır. Eğer false (varsayılan değer) ise, dışa aktarım sırasında bir özet göreve atama bulunursa bir istisna fırlatılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | kaynakların özet görevlere atanmasının dışa aktarım sırasında atlanıp atlanmayacağını belirten bir değer. |

