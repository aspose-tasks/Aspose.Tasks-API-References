---
title: "Filter"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Project içinde bir filtreyi temsil eder."
type: docs
weight: 91
url: /tr/java/com.aspose.tasks/filter/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable, com.aspose.ms.System.IEquatable
```
public final class Filter implements Comparable<Filter>, System.IEquatable<Filter>
```

Project içinde bir filtreyi temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Filter()](#Filter--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compareTo(Filter other)](#compareTo-com.aspose.tasks.Filter-) | Bu örneği, belirtilen [Filter](../../com.aspose.tasks/filter) sınıfı örneğiyle karşılaştırır ve relatif sıralarını gösteren bir değer döndürür. |
| [equals(Filter other)](#equals-com.aspose.tasks.Filter-) | Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| [equals(Object obj)](#equals-java.lang.Object-) | Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür. |
| [getCriteria()](#getCriteria--) | Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri alır. |
| [getFilterType()](#getFilterType--) | Filtrenin türünü alır. |
| [getIndex()](#getIndex--) | Filters içeren nesnedeki bir [Filter](../../com.aspose.tasks/filter) nesnesinin dizinini alır. |
| [getName()](#getName--) | Bir Filter nesnesinin adını alır. |
| [getShowInMenu()](#getShowInMenu--) | Projenin, Şeritteki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri alır. |
| [getShowRelatedSummaryRows()](#getShowRelatedSummaryRows--) | Filtre için ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değeri alır. |
| [getUid()](#getUid--) | Bir filtrenin benzersiz tanımlayıcısını alır. |
| [hashCode()](#hashCode--) | Filtre için bir karma kod değeri döndürür. |
| [op_Equality(Filter a, Filter b)](#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThan(Filter a, Filter b)](#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür. |
| [op_GreaterThanOrEqual(Filter a, Filter b)](#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [op_Inequality(Filter a, Filter b)](#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür. |
| [op_LessThan(Filter a, Filter b)](#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür. |
| [op_LessThanOrEqual(Filter a, Filter b)](#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-) | Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür. |
| [setCriteria(FilterCriteria value)](#setCriteria-com.aspose.tasks.FilterCriteria-) | Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri ayarlar. |
| [setFilterType(int value)](#setFilterType-int-) | Filtrenin türü. |
| [setName(String value)](#setName-java.lang.String-) | Bir Filter nesnesinin adını ayarlar. |
| [setShowInMenu(boolean value)](#setShowInMenu-boolean-) | Projenin, Şeritteki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri ayarlar. |
| [setShowRelatedSummaryRows(boolean value)](#setShowRelatedSummaryRows-boolean-) | Filtre için ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değeri ayarlar. |
### Filter() {#Filter--}
```
public Filter()
```


### compareTo(Filter other) {#compareTo-com.aspose.tasks.Filter-}
```
public final int compareTo(Filter other)
```


Bu örneği, belirtilen [Filter](../../com.aspose.tasks/filter) sınıfı örneğiyle karşılaştırır ve relatif sıralarını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | Bu nesneyle karşılaştırılacak belirtilen [Filter](../../com.aspose.tasks/filter) sınıfının örneği. |

**Returns:**
int - göreceli sıralarını gösteren bir gösterge.
### equals(Filter other) {#equals-com.aspose.tasks.Filter-}
```
public final boolean equals(Filter other)
```


Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| other | [Filter](../../com.aspose.tasks/filter) | Bu örnekle karşılaştırılacak belirtilen AssignmentBaseline nesnesi. |

**Returns:**
boolean - bu örnek belirtilen AssignmentBaseline nesnesine eşitse true döndürür; aksi takdirde false.
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


Bu örneğin belirtilen AssignmentBaseline nesnesine eşit olup olmadığını gösteren bir değer döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object | Bu örnekle karşılaştırılacak belirtilen AssignmentBaseline nesnesi. |

**Returns:**
boolean - bu örnek belirtilen AssignmentBaseline nesnesine eşitse true döndürür; aksi takdirde false.
### getCriteria() {#getCriteria--}
```
public final FilterCriteria getCriteria()
```


Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri alır.

**Returns:**
[FilterCriteria](../../com.aspose.tasks/filtercriteria) - the criteria that tasks or resources must meet to be displayed in MSP view.
### getFilterType() {#getFilterType--}
```
public final int getFilterType()
```


Filtrenin türünü alır.

**Returns:**
int - filtrenin türü.
### getIndex() {#getIndex--}
```
public final int getIndex()
```


Filters içeren nesnedeki bir [Filter](../../com.aspose.tasks/filter) nesnesinin dizinini alır.

**Returns:**
int - Filters içeren nesnedeki bir [Filter](../../com.aspose.tasks/filter) nesnesinin dizini.
### getName() {#getName--}
```
public final String getName()
```


Bir Filter nesnesinin adını alır.

**Returns:**
java.lang.String - bir Filter nesnesinin adı.
### getShowInMenu() {#getShowInMenu--}
```
public final boolean getShowInMenu()
```


Projenin, Şeritteki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri alır.

**Returns:**
boolean - projenin Şeritteki Görünüm sekmesindeki Filtre açılır listesinde filtre adını gösterip göstermediğini belirten bir değer.
### getShowRelatedSummaryRows() {#getShowRelatedSummaryRows--}
```
public final boolean getShowRelatedSummaryRows()
```


Filtre için ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değeri alır.

**Returns:**
boolean - filtrenin ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değer.
### getUid() {#getUid--}
```
public final int getUid()
```


Bir filtrenin benzersiz tanımlayıcısını alır.

**Returns:**
int - bir filtrenin benzersiz tanımlayıcısı.
### hashCode() {#hashCode--}
```
public int hashCode()
```


Filtre için bir karma kod değeri döndürür.

**Returns:**
int - bu nesne için bir karma kod değeri döndürür.
### op_Equality(Filter a, Filter b) {#op-Equality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Equality(Filter a, Filter b)
```


Bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olup olmadığını belirten bir değer
### op_GreaterThan(Filter a, Filter b) {#op-GreaterThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThan(Filter a, Filter b)
```


Bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük olup olmadığını belirten bir değer
### op_GreaterThanOrEqual(Filter a, Filter b) {#op-GreaterThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_GreaterThanOrEqual(Filter a, Filter b)
```


Bu örneğin belirtilen nesneden büyük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneden büyük ya da ona eşit olup olmadığını belirten bir değer
### op_Inequality(Filter a, Filter b) {#op-Inequality-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_Inequality(Filter a, Filter b)
```


Bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneye eşit olmama durumunu belirten bir değer
### op_LessThan(Filter a, Filter b) {#op-LessThan-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThan(Filter a, Filter b)
```


Bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük olup olmadığını belirten bir değer
### op_LessThanOrEqual(Filter a, Filter b) {#op-LessThanOrEqual-com.aspose.tasks.Filter-com.aspose.tasks.Filter-}
```
public static boolean op_LessThanOrEqual(Filter a, Filter b)
```


Bu örneğin belirtilen nesneden küçük veya ona eşit olup olmadığını belirten bir değeri döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| a | [Filter](../../com.aspose.tasks/filter) | İlk filtre. |
| b | [Filter](../../com.aspose.tasks/filter) | İkinci filtre. |

**Returns:**
boolean - bu örneğin belirtilen nesneden küçük ya da ona eşit olup olmadığını belirten bir değer
### setCriteria(FilterCriteria value) {#setCriteria-com.aspose.tasks.FilterCriteria-}
```
public final void setCriteria(FilterCriteria value)
```


Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FilterCriteria](../../com.aspose.tasks/filtercriteria) | MSP görünümünde görüntülenmek için görevlerin veya kaynakların karşılaması gereken kriterler. |

### setFilterType(int value) {#setFilterType-int-}
```
public final void setFilterType(int value)
```


Filtrenin türü.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | filtrenin türü. |

### setName(String value) {#setName-java.lang.String-}
```
public final void setName(String value)
```


Bir Filter nesnesinin adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | Bir Filter nesnesinin adı. |

### setShowInMenu(boolean value) {#setShowInMenu-boolean-}
```
public final void setShowInMenu(boolean value)
```


Projenin, Şeritteki Görünüm sekmesindeki Filter açılır listesinde filtre adını gösterip göstermediğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | projenin Şeritteki Görünüm sekmesindeki Filtre açılır listesinde filtre adını gösterip göstermediğini belirten bir değer. |

### setShowRelatedSummaryRows(boolean value) {#setShowRelatedSummaryRows-boolean-}
```
public final void setShowRelatedSummaryRows(boolean value)
```


Filtre için ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | filtre için ilgili özet satırlarının gösterilip gösterilmediğini belirten bir değer. |

