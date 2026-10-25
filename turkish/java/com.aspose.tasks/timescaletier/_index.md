---
title: "TimescaleTier"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Gantt Şeması'nda zaman ölçeğinin tek bir katmanını temsil eder."
type: docs
weight: 325
url: /tr/java/com.aspose.tasks/timescaletier/
---

**Inheritance:**
java.lang.Object
```
public final class TimescaleTier
```

Gantt Şeması'nda zaman ölçeğinin tek bir katmanını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [TimescaleTier()](#TimescaleTier--) | Yeni bir [TimescaleTier](../../com.aspose.tasks/timescaletier) sınıfının bir örneğini başlatır. |
| [TimescaleTier(int unit, int count)](#TimescaleTier-int-int-) | Yeni bir [TimescaleTier](../../com.aspose.tasks/timescaletier) sınıfının bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAlignment()](#getAlignment--) | Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını alır ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [getCount()](#getCount--) | Katman için etiketlerin gösterileceği zaman birimi aralığını alır. |
| [getDateTimeConverter()](#getDateTimeConverter--) | Bu katmanda tarih işaretinin render edilmesini işlemek için bir geri çağırma işlevi alır. |
| [getLabel()](#getLabel--) | Zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel) alır. |
| [getRenderLabelOnEachPage()](#getRenderLabelOnEachPage--) | Bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrağı alır. |
| [getShowTicks()](#getShowTicks--) | Katmandaki zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değeri alır. |
| [getUnit()](#getUnit--) | Zaman ölçeği katmanı için zaman ölçeği birimi [TimescaleUnit](../../com.aspose.tasks/timescaleunit) alır. |
| [getUsesFiscalYear()](#getUsesFiscalYear--) | Katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değeri alır. |
| [setAlignment(int value)](#setAlignment-int-) | Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ayarlar ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)). |
| [setCount(int value)](#setCount-int-) | Katman için etiketlerin gösterileceği zaman birimi aralığını ayarlar. |
| [setDateTimeConverter(DateTimeConverter value)](#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-) | Bu katmanda tarih işaretinin render edilmesini işlemek için bir geri çağırma işlevi ayarlar. |
| [setLabel(int value)](#setLabel-int-) | Zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel) ayarlar. |
| [setRenderLabelOnEachPage(boolean value)](#setRenderLabelOnEachPage-boolean-) | Bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrağı ayarlar. |
| [setShowTicks(boolean value)](#setShowTicks-boolean-) | Katmandaki zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setUnit(int value)](#setUnit-int-) | Zaman ölçeği katmanı için zaman ölçeği birimini [TimescaleUnit](../../com.aspose.tasks/timescaleunit) ayarlar. |
| [setUsesFiscalYear(boolean value)](#setUsesFiscalYear-boolean-) | Katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değeri ayarlar. |
### TimescaleTier() {#TimescaleTier--}
```
public TimescaleTier()
```


Yeni bir [TimescaleTier](../../com.aspose.tasks/timescaletier) sınıfının bir örneğini başlatır.

### TimescaleTier(int unit, int count) {#TimescaleTier-int-int-}
```
public TimescaleTier(int unit, int count)
```


Yeni bir [TimescaleTier](../../com.aspose.tasks/timescaletier) sınıfının bir örneğini başlatır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| unit | int | Zaman ölçeği birimi [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |
| count | int | [TimescaleUnit](../../com.aspose.tasks/timescaleunit) birimlerinin sayısı. |

### getAlignment() {#getAlignment--}
```
public final int getAlignment()
```


Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını alır ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Returns:**
int - katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).
### getCount() {#getCount--}
```
public final int getCount()
```


Katman için etiketlerin gösterileceği zaman birimi aralığını alır. Varsayılan değer 1'dir.

**Returns:**
int - katman için etiketlerin gösterileceği zaman birimi aralığı.
### getDateTimeConverter() {#getDateTimeConverter--}
```
public final DateTimeConverter getDateTimeConverter()
```


Bu katmanda tarih işaretinin render edilmesini işlemek için bir geri çağırma işlevi alır.

**Returns:**
[DateTimeConverter](../../com.aspose.tasks/datetimeconverter) - a callback function for handling rendering date tick in this tier.
### getLabel() {#getLabel--}
```
public final int getLabel()
```


Zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel) alır.

**Returns:**
int - zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel).
### getRenderLabelOnEachPage() {#getRenderLabelOnEachPage--}
```
public final boolean getRenderLabelOnEachPage()
```


Bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrağı alır. Değer 'true' ise, zaman dilimi birden fazla sayfaya yayıldığında, dönem için tarih etiketleri her sayfada render edilir. Değer 'false' ise, tarih etiketi sadece `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) özelliğinin değerine göre bir kez render edilir.

--------------------

MS Project'te eşdeğeri yoktur.

**Returns:**
boolean - bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrak.
### getShowTicks() {#getShowTicks--}
```
public final boolean getShowTicks()
```


Katmandaki zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - katmanda zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değer.
### getUnit() {#getUnit--}
```
public final int getUnit()
```


Zaman ölçeği katmanı için zaman ölçeği birimini [TimescaleUnit](../../com.aspose.tasks/timescaleunit) alır. Varsayılan değer [TimescaleUnit](../../com.aspose.tasks/timescaleunit)'dır.

**Returns:**
int - zaman ölçeği katmanı için zaman ölçeği birimi [TimescaleUnit](../../com.aspose.tasks/timescaleunit).
### getUsesFiscalYear() {#getUsesFiscalYear--}
```
public final boolean getUsesFiscalYear()
```


Katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değeri alır.

**Returns:**
boolean - katman etiketlerinin mali yıla göre temellendirilip edilmeyeceğini belirten bir değer.
### setAlignment(int value) {#setAlignment-int-}
```
public final void setAlignment(int value)
```


Katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ayarlar ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | katmanın her zaman dilimindeki etiketlerin nasıl hizalanacağını ([HorizontalStringAlignment](../../com.aspose.tasks/horizontalstringalignment)) belirler. |

### setCount(int value) {#setCount-int-}
```
public final void setCount(int value)
```


Katman için etiketlerin gösterileceği zaman birimi aralığını ayarlar. Varsayılan değer 1'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | katman için etiketlerin gösterileceği zaman birimi aralığı. |

### setDateTimeConverter(DateTimeConverter value) {#setDateTimeConverter-com.aspose.tasks.DateTimeConverter-}
```
public final void setDateTimeConverter(DateTimeConverter value)
```


Bu katmanda tarih işaretinin render edilmesini işlemek için bir geri çağırma işlevi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [DateTimeConverter](../../com.aspose.tasks/datetimeconverter) | bu katmanda tarih işaretinin render edilmesini işlemek için bir geri çağırma işlevi. |

### setLabel(int value) {#setLabel-int-}
```
public final void setLabel(int value)
```


Zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel) ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | zaman ölçeği katmanı için tarih etiketi [DateLabel](../../com.aspose.tasks/datelabel). |

### setRenderLabelOnEachPage(boolean value) {#setRenderLabelOnEachPage-boolean-}
```
public final void setRenderLabelOnEachPage(boolean value)
```


Bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrağı ayarlar. Değer 'true' ise, zaman dilimi birden fazla sayfaya yayıldığında, dönem için tarih etiketleri her sayfada render edilir. Değer 'false' ise, tarih etiketi `Alignment`([getAlignment](../../com.aspose.tasks/timescaletier\#getAlignment--)/[setAlignment(int)](../../com.aspose.tasks/timescaletier\#setAlignment-int-)) özelliğinin değerine göre yalnızca bir kez render edilir.

--------------------

MS Project'te eşdeğeri yoktur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | bir zaman dilimi birden fazla sayfaya yayıldığında tarih etiketlerinin her sayfada render edilip edilmeyeceğini tanımlayan bayrak. |

### setShowTicks(boolean value) {#setShowTicks-boolean-}
```
public final void setShowTicks(boolean value)
```


Katmandaki zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | katmanda zaman dilimlerini ayıran işaretçileri gösterip göstermeyeceğini belirten bir değer. |

### setUnit(int value) {#setUnit-int-}
```
public final void setUnit(int value)
```


Zaman ölçeği katmanı için zaman ölçeği birimini [TimescaleUnit](../../com.aspose.tasks/timescaleunit) ayarlar. Varsayılan değer [TimescaleUnit](../../com.aspose.tasks/timescaleunit)'dır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | zaman ölçeği katmanı için zaman ölçeği birimi [TimescaleUnit](../../com.aspose.tasks/timescaleunit). |

### setUsesFiscalYear(boolean value) {#setUsesFiscalYear-boolean-}
```
public final void setUsesFiscalYear(boolean value)
```


Katman etiketlerini mali yıla dayandırıp dayandırmayacağını belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | katman etiketlerinin mali yıla göre temellendirilip edilmeyeceğini belirten bir değer. |

