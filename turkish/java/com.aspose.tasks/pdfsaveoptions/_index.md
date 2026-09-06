---
title: "PdfSaveOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Proje sayfalarını PDF'ye oluştururken ek seçenekleri belirtmeye olanak tanır."
type: docs
weight: 191
url: /tr/java/com.aspose.tasks/pdfsaveoptions/
---

**Inheritance:**
java.lang.Object, [com.aspose.tasks.SimpleSaveOptions](../../com.aspose.tasks/simplesaveoptions), [com.aspose.tasks.SaveOptions](../../com.aspose.tasks/saveoptions)

**All Implemented Interfaces:**
com.aspose.tasks.SaveOptions.IReduceBottomGap, com.aspose.tasks.SaveOptions.IFontCallbacks, com.aspose.tasks.ICloneableSaveOptions
```
public class PdfSaveOptions extends SaveOptions implements SaveOptions.IReduceBottomGap, SaveOptions.IFontCallbacks, ICloneableSaveOptions
```

Proje sayfalarını PDF'ye oluştururken ek seçenekleri belirtmeye olanak tanır.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PdfSaveOptions()](#PdfSaveOptions--) | Bir belgeyi [SaveFileFormat](../../com.aspose.tasks/savefileformat) formatında kaydetmek için kullanılabilecek [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [copyOutputPropertiesFrom(SaveOptions source)](#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-) | \{@inheritDoc\} |
| [deepClone()](#deepClone--) | \{@inheritDoc\} |
| [getCompliance()](#getCompliance--) | Oluşturulan PDF belgesi için istenen uyumluluk seviyesini alır. |
| [getEncryptionDetails()](#getEncryptionDetails--) | Şifreleme ayrıntılarını alır. |
| [getFontSettings()](#getFontSettings--) | Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir. |
| [getPageSavingCallback()](#getPageSavingCallback--) | Her işlenen sayfa için çıktı akışı elde etmekte kullanılan kullanıcı tanımlı callback'i alır. |
| [getPages()](#getPages--) | Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini alır. |
| [getReduceFooterGap()](#getReduceFooterGap--) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır. |
| [getSaveToSeparateFiles()](#getSaveToSeparateFiles--) | Proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini gösteren bir değeri alır. |
| [getTextCompression()](#getTextCompression--) | Görseller dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü alır. |
| [setCompliance(int value)](#setCompliance-int-) | Oluşturulan PDF belgesi için istenen uyumluluk seviyesini ayarlar. |
| [setEncryptionDetails(PdfEncryptionDetails value)](#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-) | Şifreleme ayrıntılarını ayarlar. |
| [setPageSavingCallback(IPageSavingCallback value)](#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-) | Her render edilen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri aramayı ayarlar. |
| [setPages(List&lt;Integer&gt; value)](#setPages-java.util.List-java.lang.Integer--) | Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini ayarlar. |
| [setReduceFooterGap(boolean value)](#setReduceFooterGap-boolean-) | Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar. |
| [setSaveToSeparateFiles(boolean value)](#setSaveToSeparateFiles-boolean-) | Proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini gösteren bir değeri ayarlar. |
| [setTextCompression(int value)](#setTextCompression-int-) | Görseller dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü ayarlar. |
### PdfSaveOptions() {#PdfSaveOptions--}
```
public PdfSaveOptions()
```


Bir belgeyi [SaveFileFormat](../../com.aspose.tasks/savefileformat) formatında kaydetmek için kullanılabilecek [PdfSaveOptions](../../com.aspose.tasks/pdfsaveoptions) sınıfının yeni bir örneğini başlatır.

### copyOutputPropertiesFrom(SaveOptions source) {#copyOutputPropertiesFrom-com.aspose.tasks.SaveOptions-}
```
public void copyOutputPropertiesFrom(SaveOptions source)
```


Dahili kullanım için ayrılmıştır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [SaveOptions](../../com.aspose.tasks/saveoptions) | \{@inheritDoc\} |

### deepClone() {#deepClone--}
```
public SaveOptions deepClone()
```


Dahili kullanım için ayrılmıştır.

**Returns:**
[SaveOptions](../../com.aspose.tasks/saveoptions) - \{@inheritDoc\}
### getCompliance() {#getCompliance--}
```
public final int getCompliance()
```


Oluşturulan PDF belgesi için istenen uyumluluk seviyesini alır. Varsayılan değer [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15)'tir.

**Returns:**
int - oluşturulan PDF belgesi için istenen uyumluluk seviyesi.
### getEncryptionDetails() {#getEncryptionDetails--}
```
public final PdfEncryptionDetails getEncryptionDetails()
```


Şifreleme ayrıntılarını alır. Ayarlanmamışsa, şifreleme yapılmaz.

**Returns:**
[PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) - an encryption details.
### getFontSettings() {#getFontSettings--}
```
public final FontSettings getFontSettings()
```


Proje görünümü oluşturulurken kullanılan yazı tipi ayarlarını belirtir.

**Returns:**
[FontSettings](../../com.aspose.tasks/fontsettings) - font settings.
### getPageSavingCallback() {#getPageSavingCallback--}
```
public final IPageSavingCallback getPageSavingCallback()
```


Her işlenen sayfa için bir çıktı akışı elde etmek amacıyla kullanılan kullanıcı tanımlı geri çağırma işlevini alır. `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) seçeneği kullanıldığında geçerlidir.

**Returns:**
[IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) - a user-defined callback which is used to get an output stream for each rendered page.
### getPages() {#getPages--}
```
public final List<Integer> getPages()
```


Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini alır.

--------------------

Bu liste boşsa tüm sayfalar kaydedilir.

**Returns:**
java.util.List&lt;java.lang.Integer&gt; - proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesi.
### getReduceFooterGap() {#getReduceFooterGap--}
```
public final boolean getReduceFooterGap()
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren değeri alır.

**Returns:**
boolean - son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer.
### getSaveToSeparateFiles() {#getSaveToSeparateFiles--}
```
public final boolean getSaveToSeparateFiles()
```


Proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini gösteren bir değeri alır.

**Returns:**
boolean - proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini belirten bir değer.
### getTextCompression() {#getTextCompression--}
```
public final int getTextCompression()
```


Görseller dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü alır. Varsayılan, [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate) 'dir.

**Returns:**
int - görseller dışındaki tüm içerik akışları için kullanılacak bir sıkıştırma türü.
### setCompliance(int value) {#setCompliance-int-}
```
public final void setCompliance(int value)
```


Oluşturulan PDF belgesi için istenen uyumluluk seviyesini ayarlar. Varsayılan, [PdfCompliance.Pdf15](../../com.aspose.tasks/pdfcompliance\#Pdf15) 'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | oluşturulan PDF belgesi için istenen uyumluluk seviyesi. |

### setEncryptionDetails(PdfEncryptionDetails value) {#setEncryptionDetails-com.aspose.tasks.PdfEncryptionDetails-}
```
public final void setEncryptionDetails(PdfEncryptionDetails value)
```


Şifreleme ayrıntılarını ayarlar. Ayarlanmazsa, şifreleme uygulanmaz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PdfEncryptionDetails](../../com.aspose.tasks/pdfencryptiondetails) | bir şifreleme ayrıntısı. |

### setPageSavingCallback(IPageSavingCallback value) {#setPageSavingCallback-com.aspose.tasks.IPageSavingCallback-}
```
public final void setPageSavingCallback(IPageSavingCallback value)
```


Her işlenen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı geri çağırma ayarlar. `SaveToSeparateFiles`([getSaveToSeparateFiles()](../../com.aspose.tasks/pdfsaveoptions\#getSaveToSeparateFiles--)/[setSaveToSeparateFiles(boolean)](../../com.aspose.tasks/pdfsaveoptions\#setSaveToSeparateFiles-boolean-)) seçeneği kullanıldığında uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IPageSavingCallback](../../com.aspose.tasks/ipagesavingcallback) | Her işlenen sayfa için bir çıktı akışı almakta kullanılan kullanıcı tanımlı callback. |

### setPages(List&lt;Integer&gt; value) {#setPages-java.util.List-java.lang.Integer--}
```
public final void setPages(List<Integer> value)
```


Proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesini ayarlar.

--------------------

Bu liste boşsa tüm sayfalar kaydedilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;java.lang.Integer&gt; | proje düzeni ayrı dosyalara kaydedilirken kaydedilecek sayfa numaralarının listesi. |

### setReduceFooterGap(boolean value) {#setReduceFooterGap-boolean-}
```
public final void setReduceFooterGap(boolean value)
```


Son görev ile alt bilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Son görev ile altbilgi arasındaki boşluğun azaltılıp azaltılmayacağını gösteren bir değer. |

### setSaveToSeparateFiles(boolean value) {#setSaveToSeparateFiles-boolean-}
```
public final void setSaveToSeparateFiles(boolean value)
```


Proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini gösteren bir değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | proje sayfalarının ayrı dosyalara kaydedilip kaydedilmeyeceğini belirten bir değer. |

### setTextCompression(int value) {#setTextCompression-int-}
```
public final void setTextCompression(int value)
```


Görseller dışındaki tüm içerik akışları için kullanılacak sıkıştırma türünü ayarlar. Varsayılan, [PdfTextCompression.Flate](../../com.aspose.tasks/pdftextcompression\#Flate) 'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | görseller dışındaki tüm içerik akışları için kullanılacak bir sıkıştırma türü. |

