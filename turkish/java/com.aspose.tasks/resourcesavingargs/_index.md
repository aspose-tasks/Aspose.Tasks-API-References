---
title: "ResourceSavingArgs"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bu sınıf, HTML formatına dönüştürme sırasında gerçekleşen harici kaynak dosyalarının kaydedilmesiyle ilgili veri kümesini temsil eder."
type: docs
weight: 254
url: /tr/java/com.aspose.tasks/resourcesavingargs/
---

**Inheritance:**
java.lang.Object
```
public class ResourceSavingArgs
```

Bu sınıf, HTML formatına dönüştürme sırasında gerçekleşen dış kaynak dosyasının kaydedilmesiyle ilgili veri kümesini temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ResourceSavingArgs()](#ResourceSavingArgs--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [closeStreamIfRequired()](#closeStreamIfRequired--) | KeepStreamOpen false ise akışı kapat, aksi takdirde temizle. |
| [getFileName()](#getFileName--) | Dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adını alır. |
| [getKeepStreamOpen()](#getKeepStreamOpen--) | Kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değeri alır. |
| [getStream()](#getStream--) | Kaydedilen dosyanın ikili içeriğini alır. |
| [getUri()](#getUri--) | Kaynak URI'sını alır. |
| [setFileName(String value)](#setFileName-java.lang.String-) | Dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adını ayarlar. |
| [setKeepStreamOpen(boolean value)](#setKeepStreamOpen-boolean-) | Kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değeri ayarlar. |
| [setStream(OutputStream value)](#setStream-java.io.OutputStream-) | Kaydedilen dosyanın ikili içeriğini ayarlar. |
| [setUri(String value)](#setUri-java.lang.String-) | Kaynak URI'sını ayarlar. |
### ResourceSavingArgs() {#ResourceSavingArgs--}
```
public ResourceSavingArgs()
```


### closeStreamIfRequired() {#closeStreamIfRequired--}
```
public final void closeStreamIfRequired()
```


KeepStreamOpen false ise akışı kapat, aksi takdirde temizle.

### getFileName() {#getFileName--}
```
public final String getFileName()
```


Dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adını alır. Özel kodda dosyanın nasıl işleneceğine veya nereye kaydedileceğine karar vermek için kullanılabilir.

**Returns:**
java.lang.String - dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adı.
### getKeepStreamOpen() {#getKeepStreamOpen--}
```
public final boolean getKeepStreamOpen()
```


Kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değeri alır.

**Returns:**
boolean - kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değer.
### getStream() {#getStream--}
```
public final OutputStream getStream()
```


Kaydedilen dosyanın ikili içeriğini alır.

**Returns:**
java.io.OutputStream - kaydedilen dosyanın ikili içeriği.
### getUri() {#getUri--}
```
public final String getUri()
```


Kaynak URI'sını alır.

**Returns:**
java.lang.String - kaynak URI.
### setFileName(String value) {#setFileName-java.lang.String-}
```
public final void setFileName(String value)
```


Dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adını ayarlar. Özel kodda dosyanın nasıl işleneceğine veya nereye kaydedileceğine karar vermek için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | dönüştürücünün özel yöntem koduna gönderdiği varsayılan dosya adı. |

### setKeepStreamOpen(boolean value) {#setKeepStreamOpen-boolean-}
```
public final void setKeepStreamOpen(boolean value)
```


Kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değeri ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | kaynak kaydetme tamamlandıktan sonra akışın açık tutulup tutulmayacağını gösteren değer. |

### setStream(OutputStream value) {#setStream-java.io.OutputStream-}
```
public final void setStream(OutputStream value)
```


Kaydedilen dosyanın ikili içeriğini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.io.OutputStream | kaydedilen dosyanın ikili içeriği. |

### setUri(String value) {#setUri-java.lang.String-}
```
public final void setUri(String value)
```


Kaynak URI'sını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | kaynak URI'si. |

