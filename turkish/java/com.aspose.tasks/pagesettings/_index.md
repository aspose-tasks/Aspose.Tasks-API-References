---
title: "PageSettings"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje görünümünün bir sayfası için baskı ayarlarını temsil eder."
type: docs
weight: 181
url: /tr/java/com.aspose.tasks/pagesettings/
---

**Inheritance:**
java.lang.Object
```
public class PageSettings
```

Proje görünümünün bir sayfası için baskı ayarlarını temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PageSettings()](#PageSettings--) | Yeni bir [PageSettings](../../com.aspose.tasks/pagesettings) sınıfı örneği başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getAdjustToPercentOfNormalSize()](#getAdjustToPercentOfNormalSize--) | Belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değer alır. |
| [getFirstPageNumber()](#getFirstPageNumber--) | Baskı için ilk sayfa numarasını alır. |
| [getPagesInHeight()](#getPagesInHeight--) | Yükseklikte basılacak sayfa sayısını alır. |
| [getPagesInWidth()](#getPagesInWidth--) | Genişlikte basılacak sayfa sayısını alır. |
| [getPaperSize()](#getPaperSize--) | Kağıt boyutunu alır. |
| [getPaperSizeId()](#getPaperSizeId--) | PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayı alır. |
| [getPercentOfNormalSize()](#getPercentOfNormalSize--) | Baskıyı ayarlamak için normal boyutun yüzdesini alır. |
| [isPortrait()](#isPortrait--) | Sayfa yönünün dikey olup olmadığını gösteren bir değer alır; sayfa yönü yataysa false döndürür. |
| [setAdjustToPercentOfNormalSize(boolean value)](#setAdjustToPercentOfNormalSize-boolean-) | Belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değeri ayarlar. |
| [setFirstPageNumber(short value)](#setFirstPageNumber-short-) | Baskı için ilk sayfa numarasını ayarlar. |
| [setPagesInHeight(int value)](#setPagesInHeight-int-) | Yükseklikte basılacak sayfa sayısını ayarlar. |
| [setPagesInWidth(int value)](#setPagesInWidth-int-) | Genişlikte basılacak sayfa sayısını ayarlar. |
| [setPaperSize(int value)](#setPaperSize-int-) | Kağıt boyutunu ayarlar. |
| [setPaperSizeId(int value)](#setPaperSizeId-int-) | PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayıyı ayarlar. |
| [setPercentOfNormalSize(int value)](#setPercentOfNormalSize-int-) | Baskıyı ayarlamak için normal boyutun yüzdesini ayarlar. |
| [setPortrait(boolean value)](#setPortrait-boolean-) | Sayfa yönünün dikey olup olmadığını gösteren bir değeri ayarlar; sayfa yönü yataysa false döndürür. |
### PageSettings() {#PageSettings--}
```
public PageSettings()
```


Yeni bir [PageSettings](../../com.aspose/tasks/pagesettings) sınıfı örneği başlatır. Proje görünümünün bir sayfası için baskı ayarlarını temsil eder.

### getAdjustToPercentOfNormalSize() {#getAdjustToPercentOfNormalSize--}
```
public final boolean getAdjustToPercentOfNormalSize()
```


Belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değer alır.

--------------------

Proje HTML formatında render edildiğinde etkili değildir.

**Returns:**
boolean - belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değer.
### getFirstPageNumber() {#getFirstPageNumber--}
```
public final short getFirstPageNumber()
```


Baskı için ilk sayfa numarasını alır.

**Returns:**
short - baskı için ilk sayfa numarası.
### getPagesInHeight() {#getPagesInHeight--}
```
public final int getPagesInHeight()
```


Yükseklikte basılacak sayfa sayısını alır.

**Returns:**
int - yüksekliğinde basılacak sayfa sayısı.
### getPagesInWidth() {#getPagesInWidth--}
```
public final int getPagesInWidth()
```


Genişlikte basılacak sayfa sayısını alır.

**Returns:**
int - genişliğinde basılacak sayfa sayısı.
### getPaperSize() {#getPaperSize--}
```
public final int getPaperSize()
```


Kağıt boyutunu alır. [PrinterPaperSize](../../com.aspose/tasks/printerpapersize) enumarasyonunun değerlerinden biri olabilir.

**Returns:**
int - bir kağıt boyutu.
### getPaperSizeId() {#getPaperSizeId--}
```
public final int getPaperSizeId()
```


PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayı alır. Bu değer, OS ayarlarından PaperSize elde etmek için kullanılabilir ().

**Returns:**
int - PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayı.
### getPercentOfNormalSize() {#getPercentOfNormalSize--}
```
public final int getPercentOfNormalSize()
```


Baskıyı ayarlamak için normal boyutun yüzdesini alır.

**Returns:**
int - baskıyı ayarlamak için normal boyutun bir yüzdesi.
### isPortrait() {#isPortrait--}
```
public final boolean isPortrait()
```


Sayfa yönünün dikey olup olmadığını gösteren bir değer alır; sayfa yönü yataysa false döndürür.

--------------------

Render sırasında SaveOptions.getPageSize() == PageSize.DefinedInView olduğunda uygulanır.

**Returns:**
boolean - sayfa yönünün portre olup olmadığını gösteren bir değer; sayfa yönü manzara ise false döndürür.
### setAdjustToPercentOfNormalSize(boolean value) {#setAdjustToPercentOfNormalSize-boolean-}
```
public final void setAdjustToPercentOfNormalSize(boolean value)
```


Belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose/tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose/tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değeri ayarlar.

--------------------

Proje HTML formatında render edildiğinde etkili değildir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | boolean | belirtilen yüzdeye (`PercentOfNormalSize`([getPercentOfNormalSize()](../../com.aspose.tasks/pagesettings\#getPercentOfNormalSize--)/ [setPercentOfNormalSize(int)](../../com.aspose.tasks/pagesettings\#setPercentOfNormalSize-int-))) göre baskıyı ayarlayıp ayarlamayacağını gösteren bir değer. |

### setFirstPageNumber(short value) {#setFirstPageNumber-short-}
```
public final void setFirstPageNumber(short value)
```


Baskı için ilk sayfa numarasını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | short | baskı için ilk sayfa numarası. |

### setPagesInHeight(int value) {#setPagesInHeight-int-}
```
public final void setPagesInHeight(int value)
```


Yükseklikte basılacak sayfa sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | yükseklikte basılacak sayfa sayısı. |

### setPagesInWidth(int value) {#setPagesInWidth-int-}
```
public final void setPagesInWidth(int value)
```


Genişlikte basılacak sayfa sayısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | genişlikte basılacak sayfa sayısı. |

### setPaperSize(int value) {#setPaperSize-int-}
```
public final void setPaperSize(int value)
```


Bir kağıt boyutu ayarlar. [PrinterPaperSize](../../com.aspose.tasks/printerpapersize) enum değerlerinden biri olabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | bir kağıt boyutu. |

### setPaperSizeId(int value) {#setPaperSizeId-int-}
```
public final void setPaperSizeId(int value)
```


PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayı ayarlar. Bu değer, OS ayarlarından PaperSize elde etmek için kullanılabilir ().

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | PrinterPaperSize değerlerinden birini veya özel bir sayfa boyutu kimliğini temsil eden bir tamsayı. |

### setPercentOfNormalSize(int value) {#setPercentOfNormalSize-int-}
```
public final void setPercentOfNormalSize(int value)
```


Baskıyı ayarlamak için normal boyutun yüzdesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | baskıyı ayarlamak için normal boyutun bir yüzdesi. |

### setPortrait(boolean value) {#setPortrait-boolean-}
```
public final void setPortrait(boolean value)
```


Sayfa yönünün dikey olup olmadığını gösteren bir değeri ayarlar; sayfa yönü yataysa false döndürür.

--------------------

Render sırasında SaveOptions.getPageSize() == PageSize.DefinedInView olduğunda uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | sayfa yönünün portre olup olmadığını gösteren bir değer; sayfa yönü manzara ise false döndürür. |

