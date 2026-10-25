---
title: "PrimaveraReadOptions"
second_title: "Aspose.Tasks for Java API Referansı"
description: "Primavera Xml veya Primavera Xer dosyaları okunurken ek seçeneklerin belirtilmesine izin verir."
type: docs
weight: 206
url: /tr/java/com.aspose.tasks/primaverareadoptions/
---

**Inheritance:**
java.lang.Object
```
public class PrimaveraReadOptions
```

Primavera Xml veya Primavera Xer dosyaları okunurken ek seçeneklerin belirtilmesine izin verir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PrimaveraReadOptions()](#PrimaveraReadOptions--) | Yeni bir [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) sınıfının bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [getPreserveUids()](#getPreserveUids--) | Varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı alır. |
| [getProjectUid()](#getProjectUid--) | Birden fazla proje içeren dosyadan okunacak projenin UID'sini alır. |
| [getReadBaselineProjects()](#getReadBaselineProjects--) | Temel proje setlerinin yüklenip yüklenmeyeceğini belirten bir bayrağı alır. |
| [getUndefinedConstraintHandlingBehavior()](#getUndefinedConstraintHandlingBehavior--) | XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranışı belirtir. |
| [setPreserveUids(boolean value)](#setPreserveUids-boolean-) | Varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı ayarlar. |
| [setProjectUid(int value)](#setProjectUid-int-) | Birden fazla proje içeren dosyadan okunacak projenin UID'sini ayarlar. |
| [setReadBaselineProjects(boolean value)](#setReadBaselineProjects-boolean-) | Temel proje setlerinin yüklenip yüklenmeyeceğini belirten bir bayrağı ayarlar. |
| [setUndefinedConstraintHandlingBehavior(int value)](#setUndefinedConstraintHandlingBehavior-int-) | XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranışı belirtir. |
### PrimaveraReadOptions() {#PrimaveraReadOptions--}
```
public PrimaveraReadOptions()
```


Yeni bir [PrimaveraReadOptions](../../com.aspose/tasks/primaverareadoptions) sınıfının bir örneğini başlatır.

### getPreserveUids() {#getPreserveUids--}
```
public final boolean getPreserveUids()
```


Varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı alır.

**Returns:**
boolean - varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrak.
### getProjectUid() {#getProjectUid--}
```
public final int getProjectUid()
```


Birden fazla proje içeren dosyadan okunacak projenin UID'sini alır.

**Returns:**
int - birden fazla proje içeren dosyadan okunacak projenin UID'si.
### getReadBaselineProjects() {#getReadBaselineProjects--}
```
public final boolean getReadBaselineProjects()
```


Temel proje setlerinin yüklenip yüklenmeyeceğini belirten bir bayrağı alır. Varsayılan değer doğrudur.

--------------------

Bu bayrak, temel proje setleri içeren Primavera XML dosyalarına uygulanır (temel setler XER formatı tarafından desteklenmez). Temel veri gerekmediğinde büyük bir projenin temel setlerle yüklenmesini hızlandırmak için seçenek false olarak ayarlanabilir.

**Returns:**
boolean - temel proje setlerinin yüklenip yüklenmeyeceğini belirten bir bayrak.
### getUndefinedConstraintHandlingBehavior() {#getUndefinedConstraintHandlingBehavior--}
```
public final int getUndefinedConstraintHandlingBehavior()
```


XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranışı belirtir.

**Returns:**
int - XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranış.
### setPreserveUids(boolean value) {#setPreserveUids-boolean-}
```
public final void setPreserveUids(boolean value)
```


Varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrağı ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | varlıkların özgün benzersiz tanımlayıcılarının korunup korunmayacağını belirten bir bayrak. |

### setProjectUid(int value) {#setProjectUid-int-}
```
public final void setProjectUid(int value)
```


Birden fazla proje içeren dosyadan okunacak projenin UID'sini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | birden fazla proje içeren dosyadan okunacak projenin UID'si. |

### setReadBaselineProjects(boolean value) {#setReadBaselineProjects-boolean-}
```
public final void setReadBaselineProjects(boolean value)
```


Temel projelerin yüklenip yüklenmeyeceğini belirten bir bayrak ayarlar. Varsayılan değer true'dur.

--------------------

Bu bayrak, temel proje setleri içeren Primavera XML dosyalarına uygulanır (temel setler XER formatı tarafından desteklenmez). Temel veri gerekmediğinde büyük bir projenin temel setlerle yüklenmesini hızlandırmak için seçenek false olarak ayarlanabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean | Temel projelerin yüklenip yüklenmeyeceğini belirten bir bayrak. |

### setUndefinedConstraintHandlingBehavior(int value) {#setUndefinedConstraintHandlingBehavior-int-}
```
public final void setUndefinedConstraintHandlingBehavior(int value)
```


XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranışı belirtir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int | XER formatından okunan tanımsız kısıtlamalara sahip görevleri işlemek için kullanılan davranış. |

