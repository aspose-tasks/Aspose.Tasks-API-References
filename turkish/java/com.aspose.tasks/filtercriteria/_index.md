---
title: "FilterCriteria"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri tanımlar."
type: docs
weight: 94
url: /tr/java/com.aspose.tasks/filtercriteria/
---

**Inheritance:**
java.lang.Object
```
public class FilterCriteria
```

Görevlerin veya kaynakların MSP görünümünde görüntülenmesi için karşılaması gereken kriterleri tanımlar.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [FilterCriteria()](#FilterCriteria--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCriteriaRows()](#getCriteriaRows--) | Çocuk [FilterCriteria](../../com.aspose.tasks/filtercriteria) satırlarının listesini alır. |
| [getField()](#getField--) | Değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) alır. |
| [getOperation()](#getOperation--) | Filtredeki diğer kriterlerle ilişkili, FieldName, Test ve Value ile belirlenen kriteri alır. |
| [getTest()](#getTest--) | Filtre için seçim kriteri olarak işlev gören, FieldName ve Value arasındaki karşılaştırma türünü alır. |
| [getValues()](#getValues--) | FieldName ile belirtilen alanın değeriyle karşılaştırmak için nesne değerlerini alır. |
| [isValueAField()](#isValueAField--) | FilterCriteria'nin sağ taraf değerinin sabit bir değer değil, bir alan referansı olup olmadığını alır. |
| [isValueAField(int index)](#isValueAField-int-) | FilterCriteria'nin indeksindeki değerin sabit bir değer değil, bir alan referansı olup olmadığını alır. |
| [setField(int value)](#setField-int-) | Değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) ayarlar. |
| [setOperation(int value)](#setOperation-int-) | Filtredeki diğer kriterlerle ilişkili, FieldName, Test ve Value ile belirlenen kriteri ayarlar. |
| [setTest(int value)](#setTest-int-) | Filtre için seçim kriteri olarak işlev gören, FieldName ve Value arasındaki karşılaştırma türünü ayarlar. |
| [setValue(int index, Object value)](#setValue-int-java.lang.Object-) | FieldName tarafından belirtilen alanın değeriyle karşılaştırmak için indeksdeki nesne değerini ayarlar. |
| [setValue(Object value)](#setValue-java.lang.Object-) | FieldName tarafından belirtilen alanın değeriyle karşılaştırmak için nesne değerini ayarlar. |
| [setValueByField(int value)](#setValueByField-int-) | FieldName tarafından belirtilen alanın değeriyle karşılaştırılacak değere sahip alanı ayarlar. |
| [setValueByField(int index, int value)](#setValueByField-int-int-) | FieldName tarafından belirtilen alanın değeriyle karşılaştırılacak değere sahip, indeksdeki alanı ayarlar. |
| [toString()](#toString--) | [FilterCriteria](../../com.aspose.tasks/filtercriteria) sınıfının örneğinin dize temsilini döndürür. |
### FilterCriteria() {#FilterCriteria--}
```
public FilterCriteria()
```


### getCriteriaRows() {#getCriteriaRows--}
```
public final List<FilterCriteria> getCriteriaRows()
```


Çocuk [FilterCriteria](../../com.aspose.tasks/filtercriteria) satırlarının listesini alır. Filtre birden fazla kriter satırı içeriyorsa, And operatörünün etkisi, her iki satırın kriterlerinin de bu filtrenin sonucu olarak görev veya kaynağın görüntülenmesi için karşılanması gerektiğidir. Or operatörünün etkisi ise, satırlardan birinin kriterlerinin karşılanması gerektiğidir.

**Returns:**
java.util.List&lt;com.aspose.tasks.FilterCriteria&gt; - çocuk [FilterCriteria](../../com.aspose.tasks/filtercriteria) satırlarının listesi.
### getField() {#getField--}
```
public final int getField()
```


Değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) alır.

**Returns:**
int - değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)).
### getOperation() {#getOperation--}
```
public final int getOperation()
```


Filtredeki diğer kriterlerle ilişkili, FieldName, Test ve Value ile belirlenen kriteri alır.

**Returns:**
int - Filterdeki diğer kriterlerle ilişkili, FieldName, Test ve Value ile belirlenen kriter.
### getTest() {#getTest--}
```
public final int getTest()
```


Filtre için seçim kriteri olarak işlev gören, FieldName ve Value arasındaki karşılaştırma türünü alır. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - Filtre için seçim kriteri olarak işlev gören, FieldName ve Value arasındaki karşılaştırma türü.
### getValues() {#getValues--}
```
public final Object[] getValues()
```


FieldName ile belirtilen alanın değeriyle karşılaştırmak için nesne değerlerini alır.

**Returns:**
java.lang.Object[] - FieldName ile belirtilen alanın değeriyle karşılaştırmak için nesne değerleri.
### isValueAField() {#isValueAField--}
```
public final boolean isValueAField()
```


FilterCriteria'nin sağ taraf değerinin sabit bir değer değil, bir alan referansı olup olmadığını alır.

**Returns:**
boolean - FilterCriteria'nin sağ taraf değerinin sabit bir değer değil, bir alan referansı olup olmadığı.
### isValueAField(int index) {#isValueAField-int-}
```
public final boolean isValueAField(int index)
```


FilterCriteria'nin indeksindeki değerin sabit bir değer değil, bir alan referansı olup olmadığını alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | değerin indeksi |

**Returns:**
boolean - FilterCriteria dizinindeki sağ taraftaki değerin bir alan referansı olup olmadığını, sabit bir değer olmadığını belirtir.
### setField(int value) {#setField-int-}
```
public final void setField(int value)
```


Değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | değiştirmek için bir `Field`([getField()](../../com.aspose.tasks/filtercriteria\#getField--)/[setField(int)](../../com.aspose.tasks/filtercriteria\#setField-int-)) |

### setOperation(int value) {#setOperation-int-}
```
public final void setOperation(int value)
```


Filtredeki diğer kriterlerle ilişkili, FieldName, Test ve Value ile belirlenen kriteri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | FieldName, Test ve Value ile oluşturulan kriter, filtredeki diğer kriterlerle ilişkilidir. |

### setTest(int value) {#setTest-int-}
```
public final void setTest(int value)
```


Filtre için seçim kriteri olarak işlev gören FieldName ve Value arasındaki karşılaştırma türünü ayarlar. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Filtre için seçim kriteri olarak işlev gören FieldName ve Value arasındaki karşılaştırma türü. |

### setValue(int index, Object value) {#setValue-int-java.lang.Object-}
```
public final void setValue(int index, Object value)
```


FieldName tarafından belirtilen alanın değeriyle karşılaştırmak için indeksdeki nesne değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | değerin dizini. |
| değer | java.lang.Object | filtre kriterinin dizinindeki sağ taraftaki değer olarak kullanılacak nesne değeri. |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public final void setValue(Object value)
```


FieldName tarafından belirtilen alanın değeriyle karşılaştırmak için nesne değerini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | filtre kriterinin sağ taraftaki değeri olarak kullanılacak nesne değeri. |

### setValueByField(int value) {#setValueByField-int-}
```
public final void setValueByField(int value)
```


FieldName tarafından belirtilen alanın değeriyle karşılaştırılacak değere sahip alanı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | filtre kriterinin sağ taraftaki değeri olarak kullanılacak alan. |

### setValueByField(int index, int value) {#setValueByField-int-int-}
```
public final void setValueByField(int index, int value)
```


FieldName tarafından belirtilen alanın değeriyle karşılaştırılacak değere sahip, indeksdeki alanı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | değerin indeksi |
| değer | int | filtre kriterinin dizinindeki sağ taraftaki değer olarak kullanılacak alan. |

### toString() {#toString--}
```
public String toString()
```


[FilterCriteria](../../com.aspose.tasks/filtercriteria) sınıfının örneğinin dize temsilini döndürür.

**Returns:**
java.lang.String - bu nesnenin dize temsili.
