---
title: "LevelingOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Kaynak dengelemesinin parametrelerini belirtmeye izin verir."
type: docs
weight: 142
url: /tr/java/com.aspose.tasks/levelingoptions/
---

**Inheritance:**
java.lang.Object
```
public final class LevelingOptions
```

Kaynak dengelemesinin parametrelerini belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LevelingOptions()](#LevelingOptions--) | Yeni bir [LevelingOptions](../../com.aspose/tasks/levelingoptions) sınıfının örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Bir proje dengeleme işlemini iptal etmek için kullanılabilecek bir token alır. |
| [getFinishDate()](#getFinishDate--) | Dengeleme dönemi bitiş tarihini alır. |
| [getLevelingOrder()](#getLevelingOrder--) | Dengeleme algoritmasının aşırı tahsisli görevleri geciktirdiği sıralamayı alır. |
| [getMessageHandler()](#getMessageHandler--) | Aspose.Tasks tarafından kaynak dengeleme sırasında üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını alır. |
| [getMessageLevel()](#getMessageLevel--) | Aspose.Tasks tarafından kaynak dengeleme sırasında yayımlanan günlük mesajlarının seviyesini alır. |
| [getResources()](#getResources--) | Düzleştirilecek kaynakların listesini alır. |
| [getStartDate()](#getStartDate--) | Düzleştirme dönemi başlangıç tarihini alır. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Bir proje düzleştirme işlemini iptal etmek için kullanılabilecek bir token ayarlar. |
| [setFinishDate(Date value)](#setFinishDate-java.util.Date-) | Düzleştirme dönemi bitiş tarihini ayarlar. |
| [setLevelingOrder(int value)](#setLevelingOrder-int-) | Aşırı tahsisleri olan görevlerin düzleştirme algoritması tarafından geciktirildiği sıra. |
| [setMessageHandler(IMessageHandler value)](#setMessageHandler-com.aspose.tasks.IMessageHandler-) | Kaynak düzleştirme sırasında Aspose.Tasks tarafından üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını ayarlar. |
| [setMessageLevel(int value)](#setMessageLevel-int-) | Kaynak düzleştirme sırasında Aspose.Tasks tarafından yayımlanan günlük mesajlarının seviyesini ayarlar. |
| [setResources(List&lt;Resource&gt; value)](#setResources-java.util.List-com.aspose.tasks.Resource--) | Düzleştirilecek kaynakların listesini ayarlar. |
| [setStartDate(Date value)](#setStartDate-java.util.Date-) | Düzleştirme dönemi başlangıç tarihini ayarlar. |
### LevelingOptions() {#LevelingOptions--}
```
public LevelingOptions()
```


Yeni bir [LevelingOptions](../../com.aspose/tasks/levelingoptions) sınıfının örneğini başlatır.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Bir proje dengeleme işlemini iptal etmek için kullanılabilecek bir token alır.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project leveling operation.
### getFinishDate() {#getFinishDate--}
```
public final Date getFinishDate()
```


Düzleştirme dönemi bitiş tarihini alır. Varsayılan değer projenin bitiş tarihidir.

**Returns:**
java.util.Date - düzleştirme dönemi bitiş tarihi.
### getLevelingOrder() {#getLevelingOrder--}
```
public final int getLevelingOrder()
```


Aşırı tahsislere sahip görevlerin düzleştirme algoritması tarafından geciktirildiği sırayı alır. Aşırı tahsise neden olan ve geciktirilebilecek görevler belirlendikten sonra, hangi görevin önce geciktirileceği belirtilen sıra kullanılır.

**Returns:**
int - aşırı tahsisleri olan görevlerin düzleştirme algoritması tarafından geciktirildiği sıra.
### getMessageHandler() {#getMessageHandler--}
```
public final IMessageHandler getMessageHandler()
```


Aspose.Tasks tarafından kaynak dengeleme sırasında üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını alır.

**Returns:**
[IMessageHandler](../../com.aspose.tasks/imessagehandler) - message handler callback which can be used to intercept log messages produced by Aspose.
### getMessageLevel() {#getMessageLevel--}
```
public final int getMessageLevel()
```


Aspose.Tasks tarafından kaynak dengeleme sırasında yayımlanan günlük mesajlarının seviyesini alır.

**Returns:**
int - Aspose tarafından yayımlanan günlük mesajlarının seviyesi.
### getResources() {#getResources--}
```
public final List<Resource> getResources()
```


Düzleştirilecek kaynakların listesini alır. Eğer null ayarlanırsa, tüm proje kaynakları düzleştirilecektir.

**Returns:**
java.util.List&lt;com.aspose.tasks.Resource&gt; - düzleştirilecek kaynakların listesi.
### getStartDate() {#getStartDate--}
```
public final Date getStartDate()
```


Düzleştirme dönemi başlangıç tarihini alır. Varsayılan değer projenin başlangıç tarihidir.

**Returns:**
java.util.Date - düzleştirme dönemi başlangıç tarihi.
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Bir proje düzleştirme işlemini iptal etmek için kullanılabilecek bir token ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | Bir proje düzleştirme işlemini iptal etmek için kullanılabilecek bir token. |

### setFinishDate(Date value) {#setFinishDate-java.util.Date-}
```
public final void setFinishDate(Date value)
```


Düzleştirme dönemi bitiş tarihini ayarlar. Varsayılan değer projenin bitiş tarihidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | düzleştirme dönemi bitiş tarihi. |

### setLevelingOrder(int value) {#setLevelingOrder-int-}
```
public final void setLevelingOrder(int value)
```


Aşırı tahsisleri olan görevlerin düzleştirme algoritması tarafından geciktirildiği sıra. Aşırı tahsise neden olan ve geciktirilebilecek görevler belirlendikten sonra, hangi görevin önce geciktirileceği belirtilen sıra kullanılır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | aşırı tahsisleri olan görevlerin düzleştirme algoritması tarafından geciktirildiği sıra. |

### setMessageHandler(IMessageHandler value) {#setMessageHandler-com.aspose.tasks.IMessageHandler-}
```
public final void setMessageHandler(IMessageHandler value)
```


Kaynak düzleştirme sırasında Aspose.Tasks tarafından üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [IMessageHandler](../../com.aspose.tasks/imessagehandler) | Aspose tarafından üretilen günlük mesajlarını yakalamak için kullanılabilecek mesaj işleyici geri çağrısı. |

### setMessageLevel(int value) {#setMessageLevel-int-}
```
public final void setMessageLevel(int value)
```


Kaynak düzleştirme sırasında Aspose.Tasks tarafından yayımlanan günlük mesajlarının seviyesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | Aspose tarafından yayımlanan günlük mesajlarının seviyesi. |

### setResources(List&lt;Resource&gt; value) {#setResources-java.util.List-com.aspose.tasks.Resource--}
```
public final void setResources(List<Resource> value)
```


Düzleştirilecek kaynakların listesini ayarlar. Null ayarlanırsa, tüm proje kaynakları düzleştirilecektir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.List&lt;com.aspose.tasks.Resource&gt; | düzleştirilecek kaynakların listesi. |

### setStartDate(Date value) {#setStartDate-java.util.Date-}
```
public final void setStartDate(Date value)
```


Düzleştirme dönemi başlangıç tarihini ayarlar. Varsayılan değer projenin başlangıç tarihidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.util.Date | düzleştirme dönemi başlangıç tarihi. |

