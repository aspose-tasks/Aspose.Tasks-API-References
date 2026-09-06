---
title: "ProgressLines"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Gantt Şeması görünümünde ilerleme çizgilerini temsil eder."
type: docs
weight: 219
url: /tr/java/com.aspose.tasks/progresslines/
---

**Inheritance:**
java.lang.Object
```
public class ProgressLines
```

Gantt Şeması görünümünde ilerleme çizgilerini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ProgressLines()](#ProgressLines--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getBeginAtDate()](#getBeginAtDate--) | İlerleme çizgelerinin gösterileceği tarihi alır. |
| [getBeginAtProjectStart()](#getBeginAtProjectStart--) | Projenin başlangıç tarihinden itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır. |
| [getDateFormat()](#getDateFormat--) | Tarih biçimini alır ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [getDisplayAtCurrentDate()](#getDisplayAtCurrentDate--) | Geçerli tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır. |
| [getDisplayAtRecurringIntervals()](#getDisplayAtRecurringIntervals--) | Yinelenen aralıklarla ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır. |
| [getDisplaySelected()](#getDisplaySelected--) | Seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır. |
| [getFont()](#getFont--) | İlerleme çizgi etiketi için kullanılan yazı tipini alır. |
| [getLineColor()](#getLineColor--) | Geçerli ilerleme çizgisi için çizgi rengini alır. |
| [getLinePattern()](#getLinePattern--) | Geçerli ilerleme çizgisinin çizgi desenini alır. |
| [getOtherLineColor()](#getOtherLineColor--) | Diğer ilerleme çizgisinin rengini alır. |
| [getOtherLinePattern()](#getOtherLinePattern--) | Diğer ilerleme çizgisi için çizgi desenini alır. |
| [getOtherProgressPointColor()](#getOtherProgressPointColor--) | Diğer ilerleme noktasının rengini alır. |
| [getOtherProgressPointShape()](#getOtherProgressPointShape--) | Diğer ilerleme çizgisinin ilerleme noktasının şeklini alır. |
| [getProgressPointColor()](#getProgressPointColor--) | İlerleme noktasının rengini alır. |
| [getProgressPointShape()](#getProgressPointShape--) | İlerleme noktasının şeklini alır. |
| [getRecurringInterval()](#getRecurringInterval--) | Yinelenen aralığı alır. |
| [getSelectedDates()](#getSelectedDates--) | İlerleme çizgilerini göstermek için seçilen tarihlerin listesini alır. |
| [getShowDate()](#getShowDate--) | Her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değeri alır. |
| [isBaselinePlan()](#isBaselinePlan--) | Temel plan veya gerçek için ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır. |
| [isBaselinePlan(boolean value)](#isBaselinePlan-boolean-) | Temel plan veya gerçek için ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setBeginAtDate(Date value)](#setBeginAtDate-java.util.Date-) | İlerleme çizgilerini göstermek için başlangıç tarihini ayarlar. |
| [setBeginAtProjectStart(boolean value)](#setBeginAtProjectStart-boolean-) | Projenin başlangıç tarihinden itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setDateFormat(int value)](#setDateFormat-int-) | Tarih biçimini ayarlar ([DateLabel](../../com.aspose.tasks/datelabel)). |
| [setDisplayAtCurrentDate(boolean value)](#setDisplayAtCurrentDate-boolean-) | Geçerli tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setDisplayAtRecurringIntervals(boolean value)](#setDisplayAtRecurringIntervals-boolean-) | Yinelenen aralıklarla ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setDisplaySelected(boolean value)](#setDisplaySelected-boolean-) | Seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar. |
| [setFont(FontDescriptor value)](#setFont-com.aspose.tasks.FontDescriptor-) | İlerleme çizgi etiketi için kullanılan yazı tipini ayarlar. |
| [setLineColor(Color value)](#setLineColor-java.awt.Color-) | Mevcut ilerleme çizgisi için çizgi rengini ayarlar. |
| [setLinePattern(int value)](#setLinePattern-int-) | Mevcut ilerleme çizgisinin çizgi desenini ayarlar. |
| [setOtherLineColor(Color value)](#setOtherLineColor-java.awt.Color-) | Diğer ilerleme çizgisinin rengini ayarlar. |
| [setOtherLinePattern(int value)](#setOtherLinePattern-int-) | Diğer ilerleme çizgisi için çizgi desenini ayarlar. |
| [setOtherProgressPointColor(Color value)](#setOtherProgressPointColor-java.awt.Color-) | Diğer ilerleme noktasının rengini ayarlar. |
| [setOtherProgressPointShape(int value)](#setOtherProgressPointShape-int-) | Diğer ilerleme çizgisinin ilerleme nokta şeklini ayarlar. |
| [setProgressPointColor(Color value)](#setProgressPointColor-java.awt.Color-) | İlerleme noktasının rengini ayarlar. |
| [setProgressPointShape(int value)](#setProgressPointShape-int-) | İlerleme nokta şeklini ayarlar. |
| [setRecurringInterval(RecurringInterval value)](#setRecurringInterval-com.aspose.tasks.RecurringInterval-) | Tekrarlayan aralığı ayarlar. |
| [setShowDate(boolean value)](#setShowDate-boolean-) | Her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değeri ayarlar. |
### ProgressLines() {#ProgressLines--}
```
public ProgressLines()
```


### getBeginAtDate() {#getBeginAtDate--}
```
public final Date getBeginAtDate()
```


İlerleme çizgelerinin gösterileceği tarihi alır.

**Returns:**
java.util.Date - ilerleme çizgilerinin gösterileceği tarih.
### getBeginAtProjectStart() {#getBeginAtProjectStart--}
```
public final boolean getBeginAtProjectStart()
```


Projenin başlangıç tarihinden itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - projenin başlangıç tarihinden itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değer.
### getDateFormat() {#getDateFormat--}
```
public final int getDateFormat()
```


Tarih biçimini alır ([DateLabel](../../com.aspose.tasks/datelabel)).

**Returns:**
int - tarih biçimi ([DateLabel](../../com.aspose.tasks/datelabel)).
### getDisplayAtCurrentDate() {#getDisplayAtCurrentDate--}
```
public final boolean getDisplayAtCurrentDate()
```


Geçerli tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - mevcut tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değer.
### getDisplayAtRecurringIntervals() {#getDisplayAtRecurringIntervals--}
```
public final boolean getDisplayAtRecurringIntervals()
```


Yinelenen aralıklarla ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - tekrarlayan aralıklarda ilerleme çizgisini gösterip göstermeyeceğini belirten bir değer.
### getDisplaySelected() {#getDisplaySelected--}
```
public final boolean getDisplaySelected()
```


Seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değer.
### getFont() {#getFont--}
```
public final FontDescriptor getFont()
```


İlerleme çizgi etiketi için kullanılan yazı tipini alır.

**Returns:**
[FontDescriptor](../../com.aspose.tasks/fontdescriptor) - the font used for progress line label.
### getLineColor() {#getLineColor--}
```
public final Color getLineColor()
```


Geçerli ilerleme çizgisi için çizgi rengini alır.

**Returns:**
java.awt.Color - mevcut ilerleme çizgisi için çizgi rengi.
### getLinePattern() {#getLinePattern--}
```
public final int getLinePattern()
```


Mevcut ilerleme çizgisinin çizgi desenini alır. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Returns:**
int - mevcut ilerleme çizgisinin çizgi deseni.
### getOtherLineColor() {#getOtherLineColor--}
```
public final Color getOtherLineColor()
```


Diğer ilerleme çizgisinin rengini alır.

**Returns:**
java.awt.Color - diğer ilerleme çizgisinin rengi.
### getOtherLinePattern() {#getOtherLinePattern--}
```
public final int getOtherLinePattern()
```


Diğer ilerleme çizgisi için çizgi desenini alır.

**Returns:**
int - diğer ilerleme çizgisi için çizgi deseni.
### getOtherProgressPointColor() {#getOtherProgressPointColor--}
```
public final Color getOtherProgressPointColor()
```


Diğer ilerleme noktasının rengini alır.

**Returns:**
java.awt.Color - diğer ilerleme noktasının rengi.
### getOtherProgressPointShape() {#getOtherProgressPointShape--}
```
public final int getOtherProgressPointShape()
```


Diğer ilerleme çizgisinin ilerleme noktasının şeklini alır.

**Returns:**
int - diğer ilerleme çizgisinin ilerleme nokta şekli.
### getProgressPointColor() {#getProgressPointColor--}
```
public final Color getProgressPointColor()
```


İlerleme noktasının rengini alır.

**Returns:**
java.awt.Color - ilerleme noktasının rengi.
### getProgressPointShape() {#getProgressPointShape--}
```
public final int getProgressPointShape()
```


İlerleme noktası şeklini alır. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Returns:**
int - ilerleme noktası şekli.
### getRecurringInterval() {#getRecurringInterval--}
```
public final RecurringInterval getRecurringInterval()
```


Yineleyen aralığı alır. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Returns:**
[RecurringInterval](../../com.aspose.tasks/recurringinterval) - the recurring interval.
### getSelectedDates() {#getSelectedDates--}
```
public final List<Date> getSelectedDates()
```


İlerleme çizgilerini göstermek için seçilen tarihlerin listesini alır.

**Returns:**
java.util.List&lt;java.util.Date&gt; - ilerleme çizgileri için görüntülenecek seçilen tarihlerin listesi.
### getShowDate() {#getShowDate--}
```
public final boolean getShowDate()
```


Her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değer.
### isBaselinePlan() {#isBaselinePlan--}
```
public final boolean isBaselinePlan()
```


Temel plan veya gerçek için ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri alır.

**Returns:**
boolean - temel plan için mi yoksa gerçek için mi ilerleme çizgileri gösterileceğini belirten bir değer.
### isBaselinePlan(boolean value) {#isBaselinePlan-boolean-}
```
public final void isBaselinePlan(boolean value)
```


Temel plan veya gerçek için ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | temel plan için mi yoksa gerçek için mi ilerleme çizgileri gösterileceğini belirten bir değer. |

### setBeginAtDate(Date value) {#setBeginAtDate-java.util.Date-}
```
public final void setBeginAtDate(Date value)
```


İlerleme çizgilerini göstermek için başlangıç tarihini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | ilerleme çizgilerinin görüntüleneceği tarih. |

### setBeginAtProjectStart(boolean value) {#setBeginAtProjectStart-boolean-}
```
public final void setBeginAtProjectStart(boolean value)
```


Projenin başlangıç tarihinden itibaren ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | proje başlangıç tarihinin başından itibaren ilerleme çizgileri gösterilip gösterilmeyeceğini belirten bir değer. |

### setDateFormat(int value) {#setDateFormat-int-}
```
public final void setDateFormat(int value)
```


Tarih biçimini ayarlar ([DateLabel](../../com.aspose.tasks/datelabel)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | int | tarih formatı ([DateLabel](../../com.aspose.tasks/datelabel)). |

### setDisplayAtCurrentDate(boolean value) {#setDisplayAtCurrentDate-boolean-}
```
public final void setDisplayAtCurrentDate(boolean value)
```


Geçerli tarihte ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | geçerli tarihte ilerleme çizgisinin gösterilip gösterilmeyeceğini belirten bir değer. |

### setDisplayAtRecurringIntervals(boolean value) {#setDisplayAtRecurringIntervals-boolean-}
```
public final void setDisplayAtRecurringIntervals(boolean value)
```


Yinelenen aralıklarla ilerleme çizgisini gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | yinelenen aralıklarla ilerleme çizgisinin gösterilip gösterilmeyeceğini belirten bir değer. |

### setDisplaySelected(boolean value) {#setDisplaySelected-boolean-}
```
public final void setDisplaySelected(boolean value)
```


Seçilen tarihlerde ilerleme çizgilerini gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | seçilen tarihlerde ilerleme çizgilerinin gösterilip gösterilmeyeceğini belirten bir değer. |

### setFont(FontDescriptor value) {#setFont-com.aspose.tasks.FontDescriptor-}
```
public final void setFont(FontDescriptor value)
```


İlerleme çizgi etiketi için kullanılan yazı tipini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontDescriptor](../../com.aspose.tasks/fontdescriptor) | ilerleme çizgi etiketi için kullanılan yazı tipi. |

### setLineColor(Color value) {#setLineColor-java.awt.Color-}
```
public final void setLineColor(Color value)
```


Mevcut ilerleme çizgisi için çizgi rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | geçerli ilerleme çizgisi için çizgi rengi. |

### setLinePattern(int value) {#setLinePattern-int-}
```
public final void setLinePattern(int value)
```


Geçerli ilerleme çizgisinin çizgi desenini ayarlar. `LinePattern`([getLinePattern()](../../com.aspose.tasks/progresslines\#getLinePattern--)/[setLinePattern(int)](../../com.aspose.tasks/progresslines\#setLinePattern-int-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | geçerli ilerleme çizgisinin çizgi deseni. |

### setOtherLineColor(Color value) {#setOtherLineColor-java.awt.Color-}
```
public final void setOtherLineColor(Color value)
```


Diğer ilerleme çizgisinin rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | diğer ilerleme çizgisinin rengi. |

### setOtherLinePattern(int value) {#setOtherLinePattern-int-}
```
public final void setOtherLinePattern(int value)
```


Diğer ilerleme çizgisi için çizgi desenini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | diğer ilerleme çizgisi için çizgi deseni. |

### setOtherProgressPointColor(Color value) {#setOtherProgressPointColor-java.awt.Color-}
```
public final void setOtherProgressPointColor(Color value)
```


Diğer ilerleme noktasının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | diğer ilerleme noktasının rengi. |

### setOtherProgressPointShape(int value) {#setOtherProgressPointShape-int-}
```
public final void setOtherProgressPointShape(int value)
```


Diğer ilerleme çizgisinin ilerleme nokta şeklini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | diğer ilerleme çizgisinin ilerleme noktası şekli. |

### setProgressPointColor(Color value) {#setProgressPointColor-java.awt.Color-}
```
public final void setProgressPointColor(Color value)
```


İlerleme noktasının rengini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.awt.Color | ilerleme noktasının rengi. |

### setProgressPointShape(int value) {#setProgressPointShape-int-}
```
public final void setProgressPointShape(int value)
```


İlerleme noktası şeklini ayarlar. [GanttBarEndShape](../../com.aspose.tasks/ganttbarendshape).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | ilerleme noktası şekli. |

### setRecurringInterval(RecurringInterval value) {#setRecurringInterval-com.aspose.tasks.RecurringInterval-}
```
public final void setRecurringInterval(RecurringInterval value)
```


Yineleyen aralığı ayarlar. `RecurringInterval`([getRecurringInterval()](../../com.aspose.tasks/progresslines\#getRecurringInterval--)/[setRecurringInterval(RecurringInterval)](../../com.aspose.tasks/progresslines\#setRecurringInterval-RecurringInterval-)).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [RecurringInterval](../../com.aspose.tasks/recurringinterval) | yinelenen aralık. |

### setShowDate(boolean value) {#setShowDate-boolean-}
```
public final void setShowDate(boolean value)
```


Her ilerleme çizgisi için tarihi gösterip göstermeyeceğini belirten bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | her ilerleme satırı için tarihi gösterip göstermeyeceğini belirten bir değer. |

