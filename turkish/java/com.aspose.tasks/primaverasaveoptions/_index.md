---
title: "PrimaveraSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Projeyi Primavera XER formatına kaydederken ek seçeneklerin belirtilmesine izin verir."
type: docs
weight: 208
url: /tr/java/com.aspose.tasks/primaverasaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions)
```
public class PrimaveraSaveOptions extends SimpleSaveOptions
```

Projeyi Primavera XER formatına kaydederken ek seçeneklerin belirtilmesine izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PrimaveraSaveOptions()](#PrimaveraSaveOptions--) | [PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getActivityIdIncrement()](#getActivityIdIncrement--) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan artışı alır. |
| [getActivityIdPrefix()](#getActivityIdPrefix--) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan ön eki alır. |
| [getActivityIdSuffix()](#getActivityIdSuffix--) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan soneki alır. |
| [getRenumberActivityIds()](#getRenumberActivityIds--) | Aktivite kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değeri alır. |
| [getSkipSummaryAssignments()](#getSkipSummaryAssignments--) | Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır. |
| [setActivityIdIncrement(int value)](#setActivityIdIncrement-int-) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan artışı ayarlar. |
| [setActivityIdPrefix(String value)](#setActivityIdPrefix-java.lang.String-) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan ön eki ayarlar. |
| [setActivityIdSuffix(int value)](#setActivityIdSuffix-int-) | Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan soneki ayarlar. |
| [setRenumberActivityIds(boolean value)](#setRenumberActivityIds-boolean-) | Etkinlik kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değer ayarlar. |
| [setSkipSummaryAssignments(boolean value)](#setSkipSummaryAssignments-boolean-) | Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri ayarlar. |
### PrimaveraSaveOptions() {#PrimaveraSaveOptions--}
```
public PrimaveraSaveOptions()
```


[PrimaveraSaveOptions](../../com.aspose.tasks/primaverasaveoptions) sınıfının yeni bir örneğini başlatır.

### getActivityIdIncrement() {#getActivityIdIncrement--}
```
public final int getActivityIdIncrement()
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan artışı alır.

**Returns:**
int - etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan artış.
### getActivityIdPrefix() {#getActivityIdPrefix--}
```
public final String getActivityIdPrefix()
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan ön eki alır.

**Returns:**
java.lang.String - etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan önek.
### getActivityIdSuffix() {#getActivityIdSuffix--}
```
public final int getActivityIdSuffix()
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan soneki alır.

**Returns:**
int - etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan sonek.
### getRenumberActivityIds() {#getRenumberActivityIds--}
```
public final boolean getRenumberActivityIds()
```


Aktivite kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değeri alır.

**Returns:**
boolean - etkinlik kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değer.
### getSkipSummaryAssignments() {#getSkipSummaryAssignments--}
```
public final boolean getSkipSummaryAssignments()
```


Kaynakların özet görevlere atamalarının dışa aktarım sırasında atlanıp atlanmayacağını gösteren bir değeri alır.

Primavera yazılımı, kaynakların özet (WBS) görevlerine atanmasını desteklemez. Bu nedenle, bu tür atamaların dışa aktarılması Primavera modeline göre geçersiz bir dosyaya yol açabilir. Eğer true ise, özet görevlere atamalar dışa aktarım sırasında atlanır. Eğer false (varsayılan değer) ise, dışa aktarım sırasında bir özet göreve atama bulunursa bir istisna fırlatılacaktır.

**Returns:**
boolean - kaynakların özet görevlere atanmasının dışa aktarım sırasında atlanıp atlanmayacağını belirten bir değer.
### setActivityIdIncrement(int value) {#setActivityIdIncrement-int-}
```
public final void setActivityIdIncrement(int value)
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan artışı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan artış. |

### setActivityIdPrefix(String value) {#setActivityIdPrefix-java.lang.String-}
```
public final void setActivityIdPrefix(String value)
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan ön eki ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan önek. |

### setActivityIdSuffix(int value) {#setActivityIdSuffix-int-}
```
public final void setActivityIdSuffix(int value)
```


Aktivite kimliklerinin yeniden numaralandırılmasında kullanılan soneki ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | etkinlik kimliklerinin yeniden numaralandırılmasında kullanılan sonek. |

### setRenumberActivityIds(boolean value) {#setRenumberActivityIds-boolean-}
```
public final void setRenumberActivityIds(boolean value)
```


Etkinlik kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değer ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | etkinlik kimliklerinin yeniden numaralandırılması gerekip gerekmediğini gösteren bir değer. |

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

