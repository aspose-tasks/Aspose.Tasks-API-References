---
title: "LoadOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Bir projeyi dosyadan veya akıştan yüklerken ek yük parametreleri belirtmeye izin verir."
type: docs
weight: 148
url: /tr/java/com.aspose.tasks/loadoptions/
---

**Inheritance:**
java.lang.Object
```
public class LoadOptions
```

Bir projeyi dosyadan veya akıştan yüklerken ek yük parametreleri belirtmeye izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [LoadOptions()](#LoadOptions--) | Yeni bir [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfının bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getCancellationToken()](#getCancellationToken--) | Bir projenin yükleme işlemini iptal etmek için kullanılabilecek bir token alır. |
| [getEncoding()](#getEncoding--) | HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlamayı alır. |
| [getErrorHandler()](#getErrorHandler--) | XML ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi alır. |
| [getPassword()](#getPassword--) | Koruma şifresini alır. |
| [getPrimaveraReadOptions()](#getPrimaveraReadOptions--) | Belirtilen bir [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğini alır; bu, Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir. |
| [setCancellationToken(CancellationToken value)](#setCancellationToken-com.aspose.tasks.CancellationToken-) | Bir projenin yükleme işlemini iptal etmek için kullanılabilecek bir token ayarlar. |
| [setEncoding(Charset value)](#setEncoding-java.nio.charset.Charset-) | HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlamayı ayarlar. |
| [setErrorHandler(ParseErrorCallback value)](#setErrorHandler-com.aspose.tasks.ParseErrorCallback-) | XML ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi ayarlar. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Koruma şifresini ayarlar. |
| [setPrimaveraReadOptions(PrimaveraReadOptions value)](#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-) | Belirtilen bir [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğini ayarlar; bu, Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir. |
### LoadOptions() {#LoadOptions--}
```
public LoadOptions()
```


Yeni bir [LoadOptions](../../com.aspose.tasks/loadoptions) sınıfının bir örneğini başlatır.

### getCancellationToken() {#getCancellationToken--}
```
public final CancellationToken getCancellationToken()
```


Bir projenin yükleme işlemini iptal etmek için kullanılabilecek bir token alır.

**Returns:**
[CancellationToken](../../com.aspose.tasks/cancellationtoken) - a token which can be used to cancel a project loading operation.
### getEncoding() {#getEncoding--}
```
public final Charset getEncoding()
```


HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlamayı alır. Varsayılan kodlama UTF8'dir.

**Returns:**
java.nio.charset.Charset - HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlama.
### getErrorHandler() {#getErrorHandler--}
```
public final ParseErrorCallback getErrorHandler()
```


XML ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi alır.

**Returns:**
[ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) - a callback method to handle xml parse errors.
### getPassword() {#getPassword--}
```
public final String getPassword()
```


Koruma şifresini alır.

**Returns:**
java.lang.String - bir koruma şifresi.
### getPrimaveraReadOptions() {#getPrimaveraReadOptions--}
```
public final PrimaveraReadOptions getPrimaveraReadOptions()
```


Belirtilen bir [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğini alır; bu, Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir.

**Returns:**
[PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) - a specified instance of the [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) class which can be used to customize the behavior of loading Primavera formats (Primavera P6 XER or Primavera P6 Xml).
### setCancellationToken(CancellationToken value) {#setCancellationToken-com.aspose.tasks.CancellationToken-}
```
public final void setCancellationToken(CancellationToken value)
```


Bir projenin yükleme işlemini iptal etmek için kullanılabilecek bir token ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [CancellationToken](../../com.aspose.tasks/cancellationtoken) | Bir projenin yükleme işlemini iptal etmek için kullanılabilecek bir token. |

### setEncoding(Charset value) {#setEncoding-java.nio.charset.Charset-}
```
public final void setEncoding(Charset value)
```


HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlamayı ayarlar. Varsayılan kodlama UTF8'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.nio.charset.Charset | HTML, MPX, XER ve Primavera XML formatlarından bir projeyi okumak için kullanılan kodlama. |

### setErrorHandler(ParseErrorCallback value) {#setErrorHandler-com.aspose.tasks.ParseErrorCallback-}
```
public final void setErrorHandler(ParseErrorCallback value)
```


XML ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [ParseErrorCallback](../../com.aspose.tasks/parseerrorcallback) | xml ayrıştırma hatalarını işlemek için bir geri çağırma yöntemi. |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public final void setPassword(String value)
```


Koruma şifresini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String | bir koruma parolası. |

### setPrimaveraReadOptions(PrimaveraReadOptions value) {#setPrimaveraReadOptions-com.aspose.tasks.PrimaveraReadOptions-}
```
public final void setPrimaveraReadOptions(PrimaveraReadOptions value)
```


Belirtilen bir [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfı örneğini ayarlar; bu, Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) | Primavera formatlarını (Primavera P6 XER veya Primavera P6 Xml) yükleme davranışını özelleştirmek için kullanılabilen [PrimaveraReadOptions](../../com.aspose.tasks/primaverareadoptions) sınıfının belirtilen bir örneği. |

