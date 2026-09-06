---
title: "GraphicalIndicatorCriteria"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge ölçütünü temsil eder."
type: docs
weight: 115
url: /tr/java/com.aspose.tasks/graphicalindicatorcriteria/
---

**Inheritance:**
java.lang.Object
```
public final class GraphicalIndicatorCriteria
```

Genişletilmiş bir öznitelikle ilişkili bir grafik gösterge ölçütünü temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Yeni bir [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) türünün örneğini başlatır. |
| [GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)](#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-) | Yeni bir [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) türünün örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getImageIndex()](#getImageIndex--) | Alan kriterleri karşılandığında görüntünün indeksini alır. |
| [getRowType()](#getRowType--) | Gösterge'nin uygulanacağı satırları belirten [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum değerini alır. |
| [getTest()](#getTest--) | Genişletilmiş özniteliğin değeri ile değerler arasındaki karşılaştırma türünü alır; bu, grafik gösterge uygulaması için bir kriter olarak işlev görür. |
| [getValue1()](#getValue1--) | Genişletilmiş özniteliğin değerini test etmek için kullanılan değeri alır. |
| [getValue2()](#getValue2--) | 'IsWithin' ve 'IsNotWithin' karşılaştırma türlerinde genişletilmiş özniteliğin değerini test etmek için kullanılan ikinci değeri alır. |
| [toString()](#toString--) | [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) sınıfının örneğinin dize temsilini döndürür. |
### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value1, GraphicalIndicatorCriteriaValue value2)
```


Yeni bir [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) türünün örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum değerinin, gösterge'nin uygulanacağı satırları belirttiği değer |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) değerinin, kriter tarafından gerçekleştirilen karşılaştırma türünü belirttiği değer. |
| imageIndex | int | Alan kriterleri karşılandığında görüntülenecek resmin indeksi |
| value1 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | Koşul kontrolünde kullanılan değerler. |
| value2 | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | 'IsWithin' ve 'IsNotWithing' koşullarında koşul kontrolünde kullanılan ikinci değer (aralığın sonu). |

### GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value) {#GraphicalIndicatorCriteria-int-int-int-com.aspose.tasks.GraphicalIndicatorCriteriaValue-}
```
public GraphicalIndicatorCriteria(int rowType, int test, int imageIndex, GraphicalIndicatorCriteriaValue value)
```


Yeni bir [GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) türünün örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowType | int | [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum değerinin, gösterge'nin uygulanacağı satırları belirttiği değer |
| test | int | [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype) değerinin, kriter tarafından gerçekleştirilen karşılaştırma türünü belirttiği değer. |
| imageIndex | int | Alan kriterleri karşılandığında görüntülenecek resmin indeksi |
| value | [GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) | Koşul kontrolünde kullanılan değer. |

### getImageIndex() {#getImageIndex--}
```
public final int getImageIndex()
```


Alan kriterleri karşılandığında görüntünün indeksini alır.

**Returns:**
int - alan kriterleri karşılandığında görüntülenecek resmin indeksi.
### getRowType() {#getRowType--}
```
public final int getRowType()
```


Gösterge'nin uygulanacağı satırları belirten [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum değerini alır.

**Returns:**
int - gösterge'nin uygulanacağı satırları belirten [GraphicalIndicatorCriteriaType](../../com.aspose.tasks/graphicalindicatorcriteriatype) enum değerinin değeri.
### getTest() {#getTest--}
```
public final int getTest()
```


Genişletilmiş özniteliğin değeri ile değerler arasındaki karşılaştırma türünü alır; bu, grafik gösterge uygulaması için bir kriter olarak işlev görür. [FilterComparisonType](../../com.aspose.tasks/filtercomparisontype)

**Returns:**
int - genişletilmiş özniteliğin değeri ile değerler arasındaki karşılaştırma türü; bu, grafik gösterge uygulaması için bir kriter olarak işlev görür.
### getValue1() {#getValue1--}
```
public final GraphicalIndicatorCriteriaValue getValue1()
```


Genişletilmiş özniteliğin değerini test etmek için kullanılan değeri alır.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the value used to test extended attribute's value.
### getValue2() {#getValue2--}
```
public final GraphicalIndicatorCriteriaValue getValue2()
```


'IsWithin' ve 'IsNotWithin' karşılaştırma türlerinde genişletilmiş özniteliğin değerini test etmek için kullanılan ikinci değeri alır.

**Returns:**
[GraphicalIndicatorCriteriaValue](../../com.aspose.tasks/graphicalindicatorcriteriavalue) - the second value used to test extended attribute's value in case of 'IsWithin' and 'IsNotWithin' comparison types.
### toString() {#toString--}
```
public String toString()
```


[GraphicalIndicatorCriteria](../../com.aspose.tasks/graphicalindicatorcriteria) sınıfının örneğinin dize temsilini döndürür.

**Returns:**
java.lang.String - bu nesnenin dize temsili.
